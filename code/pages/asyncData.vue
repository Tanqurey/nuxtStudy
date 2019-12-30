<template>
  <div>
    <p>
      我的名字是{{info.name}}，
      年龄是:{{info.age}}
    </p>
    <div>
      <img src="~static/flower.jpg" alt="">
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {};
  },
  asyncData() {
    return axios.get("https://api.myjson.com/bins/ypzq4").then(res => {
      return { info: res.data };
    });
  }
};
</script>