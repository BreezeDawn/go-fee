<template>
    <div class="m-header">
        <div class="icon"></div>
        <h1 class="text">Click Music</h1>
    </div>
</template>

<script type="text/ecmascript-6">
export default {}
</script>

<style lang="stylus" scoped rel="stylesheet/stylus">
    @import "~common/stylus/variable";
    @import "~common/stylus/mixin";
    .m-header
        position relative
        height 44px
        text-align center
        color $color-theme
        font-size: 0
        .icon
            // 显示方式
            display inline-block
            vertical-align top  // link-3，（内联）元素的顶边和行内最高元素的顶边对齐
            margin-top 6px
            margin-right 9px
            // div 高宽
            width 30px
            height 32px
            // bg 高宽
            bg-image('logo')
            background-size 30px 32px
        .text
            display inline-block
            vertical-align top
            line-height 44px  // link-5，行高是指文本行基线间的垂直距离
            font-size $font-size-large  // 通过 font-size属性来设置元素中所包含文本的字体大小
</style>