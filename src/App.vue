<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Header></Header>
    <!-- <Index></Index> -->
    <router-view></router-view>
    <!-- 专门配合路由的标签 -->
    <Footer></Footer>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Header from "./components/Header";
// import Index from "./pages/Index"
import { router } from "./routes/router";
import Footer from "./components/Footer";

export default {
  name: "app",
  components: {
    // HelloWorld
    Header,
    // Index,
    Footer
  },
  router
};
</script>

<style>
/* 引入css样式,使用@import */
@import "./assets/css/common.css";
@import "./assets/css/mycss.css";
</style>
