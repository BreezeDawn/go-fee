<template>
  <div id="app">
    <m-header></m-header>
    <tab></tab>
    <router-view></router-view>
  </div>
</template>

<script type="text/ecmasript-6">
import MHeader from 'components/m-header/m-header'
import Tab from 'components/tab/tab'
export default {
  components: {
    MHeader,
    Tab
  }
}
</script>

<style lang="stylus" scoped rel="stylesheet/stylus">
</style>
