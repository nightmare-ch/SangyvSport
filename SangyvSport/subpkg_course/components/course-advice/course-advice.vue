<template>
  <view class="course-advice-container">
    <view class="course-advice-box">
      <view class="course-advice-item">
        <text class="advice-title">时间</text>
        <text class="advice-disc">每天9分钟</text>
      </view>
      <view class="course-advice-item">
        <text class="advice-title">次数</text>
        <text class="advice-disc">4次</text>
      </view>
      <view class="course-advice-item">
        <text class="advice-title">难度</text>
        <view class="advice-pic-box">
          <image
            class="star"
            src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/黄星星.png"
            mode="scaleToFill"
          />
          <image
            class="star"
            src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/黄星星.png"
            mode="scaleToFill"
          />
          <image
            class="star"
            src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/黄星星.png"
            mode="scaleToFill"
          />
          <image
            class="star"
            src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/灰星星.png"
            mode="scaleToFill"
          />
          <image
            class="star"
            src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/灰星星.png"
            mode="scaleToFill"
          />
        </view>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  name: "course-advice",
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.course-advice-container {
  .course-advice-box {
    margin-top: 15rpx;
    .course-advice-item {
      display: inline-block;
      box-sizing: border-box;
      .advice-title {
        display: block;
        color: #818d8d;
        font-size: 24rpx;
      }
      .advice-disc {
        font-size: 36rpx;
        font-weight: bold;
      }
      .advice-pic-box {
        .star {
          width: 30rpx;
          height: 30rpx;
          margin-right: 3px;
        }
      }
    }
    .course-advice-item:nth-child(even) {
      margin: 0 155rpx 0rpx 100rpx;
    }
  }
}
</style>
