<template>
  <div id="app">
    <global-loading :imgs="['aaa.jpg']"></global-loading>
    <a class="a_link_dream"></a>
  </div>
</template>

<script>
  import GlobalLoading from './loading/globalLoading'
export default {
  name: 'app',
  data () {
    return {}
  },
  components:{
    GlobalLoading
  }
}
</script>

<style lang="less" scoped>
  @import './assets/styles/Obo.less';
  div {

  }
</style>
