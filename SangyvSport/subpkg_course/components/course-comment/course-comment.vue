<template>
  <view class="course-comment-container">
    <view class="course-comment-box">
      <text class="comment-title">优选评论</text>
      <view class="comment-title-box">
        <view class="title-data-box">
          <text class="comment-data">91%</text>
          <text class="comment-total">(共323人评价)</text>
        </view>
        <text class="comment-txt">的人认为锻炼20次后有明显效果！</text>
      </view>

      <view class="course-comment-item">
        <image
          class="user-pic"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/用户头像1.png"
          mode="scaleToFill"
        />
        <view class="user-comment-info-box">
          <text class="user-name">静待花开</text>
          <text class="user-comment"
            >朋友推荐来的，吃完早餐做完再去上班，活力满满！</text
          >
        </view>
      </view>
      <view class="course-comment-item">
        <image
          class="user-pic"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/用户头像2.png"
          mode="scaleToFill"
        />
        <view class="user-comment-info-box">
          <text class="user-name">天天</text>
          <text class="user-comment">起床必做！早上做完整个人都精神了哈哈</text>
        </view>
      </view>
      <view class="course-comment-item">
        <image
          class="user-pic"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程详情/用户头像3.png"
          mode="scaleToFill"
        />
        <view class="user-comment-info-box">
          <text class="user-name">杨丽</text>
          <text class="user-comment">锻炼完特别舒服～</text>
        </view>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  name: "course-comment",
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.course-comment-container {
  .course-comment-box {
    margin-top: 45rpx;
    box-sizing: border-box;
    .comment-title {
      font-size: 24rpx;
      color: #818d8d;
      display: flex;
    }
    .comment-title-box {
      width: 683rpx;
      height: 176rpx;
      box-sizing: border-box;
      padding: 48rpx 45rpx 0 45rpx;
      .title-data-box {
        display: inline-block;
        padding-right: 45rpx;
        .comment-data {
          font-size: 48rpx;
          color: #f7b733;
          font-weight: bold;
          padding-left: 15px;
          display: flex;
        }
        .comment-total {
          font-size: 24rpx;
          color: #f7b733;
          font-weight: bold;
        }
      }
      .comment-txt {
        display: inline-block;
        width: 385rpx;
        height: 100rpx;
        font-size: 36rpx;
      }
    }
    .course-comment-item {
      box-sizing: border-box;
      height: 130rpx;
      margin-top: 25rpx;
      position: relative;
      border-bottom: 1px solid #d8d8d8;
      .user-pic {
        width: 102rpx;
        height: 102rpx;
      }
      .user-comment-info-box {
        position: absolute;
        top: 0;
        left: 130rpx;
        .user-name {
          font-size: 24rpx;
        }
        .user-comment {
          font-size: 24rpx;
          margin-top: 10rpx;
          display: flex;
        }
      }
    }
  }
}
</style>
