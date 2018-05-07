<template>
  <div id="app">
    <hearder class="hearder"></hearder>
    <nav class="nav"></nav>
    <router-view class="main"></router-view>
  </div>
</template>

<script>
  import  nav from './views/nav'
  import  hearder from './views/hearder'
  export default {
    name: 'App',
    components: {
      hearder,
      nav,
      //注册子组件
    },
}
</script>

<style>
  *{
    padding:0;
    margin: 0;
  }
  body,html{
    position: relative;
  }
  .hearder{
    width: 100%;
    height: 20px;
    background: red;
  }
  .nav{
    margin: 0 !important;
    height: 1000px;
    width: 90px;
    background: #666666;
  }
  .main{
    width: calc(100% - 90px) !important;
    height: 1000px;
    position: absolute;
    top: 20px;
    left: 90px;
    background: #0b94ea;
  }
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
