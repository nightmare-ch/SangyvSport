<template>
  <view class="course-title-container">
    <view class="course-title-box">
      <text class="course-title">晨起唤醒活力活动</text>
      <image
        class="expert-argu"
        src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/专家认证标志.png"
        mode="scaleToFill"
      />
    </view>
  </view>
</template>

<script>
export default {
  name: "course-title",
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.course-title-container {
  .course-title-box {
    box-sizing: border-box;
    .course-title {
      font-size: 55rpx;
      font-weight: bold;
    }
    .expert-argu {
      width: 208rpx;
      height: 47rpx;
      padding-left: 5px;
    }
  }
}
</style>
