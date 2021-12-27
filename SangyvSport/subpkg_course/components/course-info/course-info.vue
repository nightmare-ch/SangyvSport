<template>
  <view class="course-info-container">
    <view class="course-pic-box">
      <image
        class="course-pic"
        src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/课程详情页-晨起唤醒.jpg"
        mode="scaleToFill"
      />
    </view>
    <view class="course-disc-container">
      <course-title></course-title>
      <course-advice></course-advice>
      <course-disc></course-disc>
      <course-comment></course-comment>
    </view>
    <course-tag></course-tag>
  </view>
</template>

<script>
import courseAdvice from '../course-advice/course-advice.vue';
import CourseComment from '../course-comment/course-comment.vue';
import CourseDisc from '../course-disc/course-disc.vue';
import CourseTag from '../course-tag/course-tag.vue';
export default {
  components: { courseAdvice, CourseDisc, CourseComment, CourseTag },
  name: "course-info",
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.course-info-container {
  .course-pic-box {
    .course-pic {
      width: 750rpx;
      height: 423rpx;
    }
  }
  .course-disc-container {
    position: absolute;
    width: 750rpx;
    top: 378rpx;
    border-radius: 57rpx 57rpx 0 0;
    background-color: white;
    padding: 45rpx 45rpx 0rpx 45rpx;
    box-sizing: border-box;
    height: 750px;
  }
}
</style>
