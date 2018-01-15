<template>
  <div :class="prefixCls">
    <div :class="" v-for="s in data.son">{{s}}</div>
  </div>
</template>

<script>
  export default {
    name: "bottom-nav",
    props: {
      prefixCls: {
        type: String,
        default: 'bottom-nav'
      },
      data: {
        type: Object
      }
    },
    computed: {
      sonClasss() {
        return [
          `${this.prefixCls}-son`
        ]
      }
    }
  }
</script>

<style lang="scss">
  $prefixCls: 'bottom-nav';

  $prefixCls{

  }
</style>
