<template>
  <view class="user-info-container">
    <view class="user-sport-info-box">
      <view class="user-sport-info-item">
        <text class="num-txt">35</text>
        <text class="unit-txt">分钟</text>
        <text class="total-txt">总运动时长</text>
      </view>
      <view class="user-sport-info-item">
        <text class="num-txt">4</text>
        <text class="unit-txt">天</text>
        <text class="total-txt">总运动天数</text>
      </view>
      <view class="user-sport-info-item">
        <text class="num-txt">12</text>
        <text class="unit-txt">次</text>
        <text class="total-txt">总运动次数</text>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  name: "user-info",
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.user-info-container {
  .user-sport-info-box {
    .user-sport-info-item {
      display: inline-block;
      padding-top: 26rpx;
      box-sizing: border-box;
      text-align: center;
      position: relative;
      .num-txt {
        color: #F7B733;
        font-size: 60rpx;
        display: inline-block;
        margin-right: 5rpx;
      }
      .unit-txt {
        font-size: 24rpx;
      }
      .total-txt {
        display: flex;
        font-size: 32rpx;
      }
    }
    .user-sport-info-item:nth-child(1) {
      margin-left: 52rpx;
      padding-right: 32rpx;
    }
    .user-sport-info-item:nth-child(even) {
      margin: 0 58rpx;
    }
    .user-sport-info-item:nth-child(3) {
      padding-left: 20rpx;
    }
    .user-sport-info-item:nth-child(1)::after {
      content: " ";
      border-left: 1px solid #d8d8d8;
      display: inline-block;
      height: 72rpx;
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      right: 0;
    }
    .user-sport-info-item:nth-child(3)::before {
      content: " ";
      border-left: 1px solid #d8d8d8;
      display: inline-block;
      height: 72rpx;
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      left: 0;
    }
  }
}
</style>
