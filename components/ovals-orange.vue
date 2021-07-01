<template>
  <div class="absolute orange-ovals w-100">
    <div class="relative h-100">
      <img src="/orange-ovals/left.png" class="orange-ovals-item orange-ovals-left">
      <img src="/orange-ovals/center.png" class="orange-ovals-item orange-ovals-center">
      <img src="/orange-ovals/right-top.png" class="orange-ovals-item orange-ovals-right-top">
      <img src="/orange-ovals/right-bottom.png" class="orange-ovals-item orange-ovals-right-bottom">
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
.orange-ovals{
  height: 200px;
  top: 150px;
  max-width: 375px;
  margin: 0 auto;
  &-item{
    position: absolute;
  }
  &-left{
    bottom: 0;
    left: 15px;
  }
  &-center{
    top: 115px;
    left: 142px;
  }
  &-right{
    &-top{
      top: 10px;
      right: 65px;
    }
    &-bottom{
      bottom: 30px;
      right: 65px;
    }
  }
}
</style>