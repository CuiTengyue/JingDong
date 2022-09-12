<template>
  <div class="docker">
    <!-- BEM   block__element--Modifier -->
    <div class="docker__item docker__item--active">
      <div class="iconfont">&#xe612;</div>
      <div class="docker__title">首页</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe67e;</div>
      <div class="docker__title">购物车</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe713;</div>
      <div class="docker__title">订单</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe78b;</div>
      <div class="docker__title">我的</div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped lang="scss">
.docker {
  display: flex; //均分等份
  position: absolute;
  box-sizing: border-box;
  padding: 0 0.18rem;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 0.49rem;
  border-top: 1px solid #f1f1f1;
  background-color: pink;
  // 1
  &__item {
  flex: 1;
  text-align: center;
  .iconfont {
    margin: 0.07rem 0 0.02rem 0;
    font-size: 0.18rem;
  }
  &--active {
    color:#1FA4FC
  }
  
}
  &__title {
  font-size: .2rem;  // 浏览器字体大小必须得10px以上
  transform:  scale(.5 , .5);  //缩小一半
  transform-origin: center top; // 参考点
}
}


</style>
