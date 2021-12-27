<template>
  <view class="TrainTimes-container">
    <text class="congrate"> 恭喜您 
      完成了第7次训练 </text>
      <image
      class="bgimage"
      src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程完成/课程完成.jpg"
      mode="widthFix"
      />
  </view>
</template>

<script>
export default {
  name: "trainTimes",
  data() {
    return {};
  },
};
</script>

<style lang="scss">
.TrainTimes-container {
  .bgimage {
    width: 100vw;
    z-index: -10;
    margin-top: -88rpx;
  }
  .congrate {
    position: absolute;
    top: 51rpx;
    padding-left: 51rpx;
    z-index: 1;
    font-size: 60rpx;
    color: white;
    font-weight: 550;
    text-shadow: grey 2px 2px 1px;
    line-height: 100rpx;
  }
}
</style>
