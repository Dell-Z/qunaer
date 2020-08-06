<template>
  <div>
    <div class="header">
      <div class="header-left">
        <div class="iconfont back-icon">&#xe624;</div>
      </div>
      <div class="header-input">
        <span class="iconfont iconType">&#xe632;</span>
        搜索</div>
      <div class="header-right">
        城市
        <span class="iconfont city-icon">&#xe6aa;</span>
      </div>  
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>
<style lang="stylus" scoped>
@import "~@/assets/styles/varibles.styl"
.header
  display: flex
  height: 0.86rem
  background: $bgColor
  color: #fff
  .header-left
    width: 0.64rem
    float: left
    line-height: 0.86rem
    .back-icon
      text-align: center
      font-size: .4rem
  .header-input
    flex: 1
    height: 0.64rem
    line-height: 0.64rem
    margin-left: 0.2rem
    margin-top: 0.12rem
    padding-left .2rem
    background-color: #fff
    border-radius: 0.1rem
    color: #ccc
    placeholder: '搜查'
    .iconType
      vertical-align top
  .header-right
    width: 1.24rem
    line-height: 0.86rem
    float: right
    text-align: center
    .city-icon
      margin-left -.1rem
      vertical-align top
</style>
