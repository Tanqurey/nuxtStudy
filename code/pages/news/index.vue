<template>
  <div>
    <h2>news index</h2>
    <ul>
      <li>
        <!-- 路由导航跳转 -->
        <nuxt-link :to="{name:'index'}">HOME</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name:'about',params:{id:'1234'}}">about</nuxt-link>
      </li>
    </ul>
    <h2>新闻列表</h2>
    <ul>
      <li>
        <nuxt-link :to="{name:'news-id',params:{id:123,title:'新闻1详细内容'}}">新闻1</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="'news/'+456">新闻2</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="'news/'+'aaa'">新闻3</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  transition: "test"
};
</script>