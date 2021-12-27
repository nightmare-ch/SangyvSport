<template>
  <view class="course-disc-container">
    <view class="course-disc-box">
      <view class="course-disc-item">
        <image
          class="disc-pic"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/笑脸.png"
          mode="scaleToFill"
        />
        <text class="disc-txt">课程效果：预热全身肌肉关节，让一天精力充沛</text>
      </view>
      <view class="course-disc-item">
        <image
          class="disc-pic"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/目标.png"
          mode="scaleToFill"
        />
        <text class="disc-txt">针对人群/问题：晨起疲乏，精力不足人群</text>
      </view>
      <view class="course-disc-item">
        <image
          class="disc-pic"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/频次.png"
          mode="scaleToFill"
        />
        <text class="disc-txt">运动频次：建议每周3~4次</text>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  name: "course-disc",
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.course-disc-container {
  .course-disc-box {
    margin-top: 42rpx;
    .course-disc-item {
      margin-bottom: 20rpx;
      position: relative;
      .disc-pic {
        width: 40rpx;
        height: 40rpx;
        padding-right: 10rpx;
        position: absolute;
        top: 0;
      }
      .disc-txt {
        width: 613rpx;
        display: flex;
        margin-left: 55rpx;
      }
    }
  }
}
</style>
