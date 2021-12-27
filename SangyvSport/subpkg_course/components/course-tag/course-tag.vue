<template>
  <view class="course-tag-container">
    <view class="course-tag-box">
      <view class="course-button">
        <text class="button-txt">开始课程</text>
      </view>
      <view class="course-att">
        <image
          class="att-pic"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/关注.png"
          mode="scaleToFill"
        />
        <text class="att-txt">关注</text>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  name: "course-tag",
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.course-tag-container {
  .course-tag-box {
    position: fixed;
    z-index: 99;
    height: 100rpx;
    bottom: 0;
    background-color: $uni-bg-color-grey;
    width: 750rpx;
    box-sizing: border-box;
    .course-button {
      width: 425rpx;
      height: 77rpx;
      background-color: #f9842d;
      text-align: center;
      line-height: 77rpx;
      border-radius: 50rpx;
      position: absolute;
      left: 148rpx;
      top: 5px;
      .button-txt {
        font-size: 36rpx;
        color: white;
      }
    }
    .course-att {
      position: absolute;
      left: 635rpx;
      top: 5px;
      .att-pic {
        width: 48rpx;
        height: 41rpx;
      }
      .att-txt {
        font-size: 24rpx;
        color: #9d9d9d;
        display: flex;
      }
    }
  }
}
</style>
