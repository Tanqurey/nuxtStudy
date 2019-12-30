<template>
  <div>
    <h2>新闻内容</h2>
    <p>新闻的id是：{{$route.params.id}}</p>
  </div>
</template>

<script>
export default {
  validate({params}) {
    // 进行路由校验
    return /^\d+$/.test(params.id);
  },
  data(){
    return {
      title:this.$route.params.title
    }
  },
  head(){
    // 覆盖父级配置
    return {
      title:this.title,
      meta:[
        {hid:'description',name:'news1',content:'新闻1内容'}
      ]
    }
  }
};
</script>