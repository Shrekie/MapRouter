<template>

  <view class="container">
    <slot></slot>
  </view>

</template>

<style>

.container {
  position: absolute;
  top: 0;

  width: 100%;
  height: 25%;

  padding:15px;
  padding-top:11%;
  background-color:rgba(0, 0, 0, 0.7);
}

</style>
