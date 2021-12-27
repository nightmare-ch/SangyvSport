<template>
  <view class="HomePage-container">
    <view class="test-button-box">
      <view class="test-button" @click="onToCourseDetail">测试按钮</view>
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    onToCourseDetail() {
      uni.navigateTo({ url: "../../subpkg_course/pages/CourseDetail/CourseDetail" });
    },
  },
};
</script>

<style lang="scss" scoped>
.HomePage-container {
  .test-button-box {
    margin-top: 100px;
    .test-button {
      width: 100px;
      height: 25px;
      background-color: #bfbfbf;
      margin: 0 auto;
      text-align: center;
    }
  }
}
</style>