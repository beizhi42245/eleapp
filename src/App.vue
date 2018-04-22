<template>
  <div id="app">
    <v-header></v-header>
    <div class="tab">
      <div class="tab-item">
        <router-link to="/">商品</router-link>
      </div>
      <div class="tab-item">
        <router-link to="/ratings">评价</router-link>
      </div>
      <div class="tab-item">
        <router-link to="/seller">商家</router-link>
      </div>      
    </div>
    <div class="content">
      我是内容
    </div>
  </div>
</template>

<script>
import Header from './components/header/header.vue'
export default {
  name: 'App',
  components: {
    'v-header': Header
  }
}
</script>

<style lang="stylus">
#app 
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  .tab
    display -webkit-box
    -webkit-box-flex: 3
    .tab-item
      display -webkit-box
      -webkit-box-flex: 1
      -webkit-box-pack center
</style>
