<template>
  <div>
    <h2>about index</h2>
    <p>传过来的数据id是：{{$route.params.id}}</p>
    <ul>
      <li>
        <!-- 路由导航跳转 -->
        <nuxt-link :to="{name:'index'}">HOME</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name:'news'}">news</nuxt-link>
      </li>
    </ul>
  </div>
</template>