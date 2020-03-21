<template>
  <div id="app">
    <router-view />
    <ul class="footer-bar">
      <li class="footer-bar-item">
        <router-link to="/">首页</router-link>
      </li>
      <li class="footer-bar-item">
        <router-link to="/category">分类</router-link>
      </li>
      <li class="footer-bar-item">
        <router-link to="/cart">购物车</router-link>
      </li>
      <li class="footer-bar-item">
        <router-link to="/profile">我的</router-link>
      </li>
    </ul>
  </div>
</template>

<style lang="scss">
.footer-bar {
  display: flex;
  background: #cccccc;
  position: fixed;
  bottom: 0;
  width: 100%; //固定定位脱离文档流
  height: 1rem;
  line-height: 1rem;
  &-item {
    //sass 语法  子元素
    flex-grow: 1;
    text-align: center;
  }
}
</style>
