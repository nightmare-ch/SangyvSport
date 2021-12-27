<template>
  <view class="user-profile-container">
    <view class="profile-box">
      <image
        class="user-photo"
        src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/我的/profile-photo.png"
        mode="scaleToFill"
      />
      <text class="user-name">榆小晚</text>
      <view class="user-title-box">
        <text class="user-title">运动小将</text>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  name: "user-profile",
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.user-profile-container {
  .profile-box {
    height: 278rpx;
    .user-photo {
      width: 167rpx;
      height: 167rpx;
      position: absolute;
      top: 67rpx;
      left: 52rpx;
    }
    .user-name {
      font-size: 48rpx;
      font-weight: bold;
      position: absolute;
      top: 105rpx;
      left: 250rpx;
    }
    .user-title-box {
      width: 147rpx;
      height: 45rpx;
      position: absolute;
      top: 165rpx;
      left: 250rpx;
      background-color: #F9842D;
      border-radius: 34rpx;
      text-align: center;
      line-height: 45rpx;
      .user-title {
        color: white;
        font-size: 24rpx;
      }
    }
  }
}
</style>
