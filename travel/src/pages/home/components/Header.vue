<template>
  <div class="header">
    <div class="header-left">返回</div>
    <div class="header-input">输入城市/景点/游玩主题</div>
    <div class="header-right">城市</div>
  </div>
</template>
<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang="stylus" scoped>
.header
  display flex
  background #00bcd4
  line-height 0.86rem
  color #fff
  .header-left
    width .64rem
    // float left
  .header-input
    flex 1
    height 0.64rem
    line-height .64rem
    margin-top .12rem
    margin-left .2rem
    background #ffffff
    border-radius .1rem
    color #cccccc
  .header-right
    // float right
    width 1.24rem
    text-align center
</style>
