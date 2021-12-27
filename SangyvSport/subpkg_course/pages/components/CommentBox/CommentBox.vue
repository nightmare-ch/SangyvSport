<template>
  <view class="comment-box">
    <uni-easyinput
      class="inputBox"
      v-if="showCommentHolder"
      ref="Comment"
      autoHeight
      type="textarea"
      prefixIcon="chat"
      suffixIcon="chat"
      v-model="value"
      placeholder="分享一下感受吧~"
      @pubComment="pubComment"
    ></uni-easyinput>
    <view class="comment-box show-comment-box" v-if="!showCommentHolder">
      <text class="myComment">我的评价</text>
      <text class="CommentConent">{{ commentContent }}</text>
    </view>
  </view>
</template>

<script>
export default {
  name: "CommentBox",
  props: {},
  data() {
    return {
      commentContent: "",
      showCommentHolder: "true",
    };
  },
  computed: {},
  methods: {
    pubComment(commentContent1) {
      if (commentContent1.split(" ").join("").length === 0) {
        uni.showToast({
          title: "发布的评论不能为空",
          icon: "none",
          duration: 2000,
        });
      } else {
        uni.showToast({
          title: "评论成功,谢谢!",
          icon: "none",
          duration: 2000,
        });
        this.showCommentHolder = !this.showCommentHolder;
        console.log(commentContent1);
        this.commentContent = commentContent1;
        this.$refs.Comment.val = "";
      }
    },
  },
  watch: {},

  // 组件周期函数--监听组件挂载完毕
  mounted() {},
  // 组件周期函数--监听组件数据更新之前
  beforeUpdate() {},
  // 组件周期函数--监听组件数据更新之后
  updated() {},
  // 组件周期函数--监听组件激活(显示)
  activated() {},
  // 组件周期函数--监听组件停用(隐藏)
  deactivated() {},
  // 组件周期函数--监听组件销毁之前
  beforeDestroy() {},
};
</script>

<style lang="scss">
.comment-box {
  display: flex;
  flex-direction: column;
  .inputBox {
    border-radius: 28.5rpx;
    margin: 44rpx 30rpx;
  }
  .show-comment-box {
    margin: 28rpx 44rpx;
    .myComment {
      font-size: 48rpx;
      font-weight: 550;
    }
    .CommentConent {
      margin-top: 28rpx;
      font-size: 40rpx;
      text-align: center;
    }
  }
}
</style>
