<template>
  <div class="tab">
    <!-- link-6 -->
    <router-link tag="div" class="tab-item" :key="tab.span" :to="tab.path" v-for="tab in tabs">
      <span class="tab-link">{{ tab.span }}</span>
    </router-link>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  data() {
    return {
      tabs: [
        { span: '推荐', path: '/recommend' },
        { span: '歌手', path: '/singer' },
        { span: '排行', path: '/rank' },
        { span: '搜索', path: '/search' }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped rel="stylesheet/stylus">
@import '~common/stylus/variable'
.tab
  display flex  // link-7
  height 44px
  line-height 44px
  font-size $font-size-medium
  .tab-item
    flex 1
    text-align center
    .tab-link
      padding-bottom 5px
      color $color-text-l
    &.router-link-active
      .tab-link
        color $color-theme
        border-bottom 2px solid $color-theme
</style>