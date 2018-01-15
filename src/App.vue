<template>
  <div id="app">
    <component :key="index" v-for="(data,index) in shopPageData" :data="data.data" :is="data.component"></component>
  </div>
</template>

<script>
  import shopPageData from './pages/shop'
  import {JBottomNav, JSearch} from '../index'

  export default {
    name: 'app',
    components: {JBottomNav, JSearch},// 这里可以一次性把所有组件导入，也可以选择部分导入
    data() {
      return {
        shopPageData
      }
    }
  }
</script>

<style lang="scss">
</style>
