<template>
  <view class="pageBox">
    <trainTimes></trainTimes>
    <view class="contentBox">
      <view class="insideBox">
        <TrainTimeShow></TrainTimeShow>
        <view class="grey"></view>
        <TrainFeeling></TrainFeeling>
        <CommentBox></CommentBox>
        
        
        <view class="buttons"></view>
        
      </view>
    </view>
  </view>
</template>

<script>
import CommentBox from "@/subpkg_course/pages/components/CommentBox/CommentBox.vue";
import TrainFeeling from "@/subpkg_course/pages/components/TrainFeeling/TrainFeeling.vue";
import trainTimes from "@/subpkg_course/pages/components/trainTimes/trainTimes.vue";
import TrainTimeShow from "@/subpkg_course/pages/components/TrainTimeShow/TrainTimeShow.vue";
import AppVue from '../../../App.vue';
export default {
  components: {
    TrainFeeling,
    TrainTimeShow,
    trainTimes,
    CommentBox
  },
  data: () => ({}),
  computed: {},
  methods: {},
  watch: {},

  // 页面周期函数--监听页面加载
  onLoad() {},
  // 页面周期函数--监听页面初次渲染完成
  onReady() {},
  // 页面周期函数--监听页面显示(not-nvue)
  onShow() {},
  // 页面周期函数--监听页面隐藏
  onHide() {},
  // 页面周期函数--监听页面卸载
  onUnload() {},
  // 页面处理函数--监听用户下拉动作
  onPullDownRefresh() {
    uni.stopPullDownRefresh();
  },
  // 页面处理函数--监听用户上拉触底
  onReachBottom() {},
  // 页面处理函数--监听页面滚动(not-nvue)
  /* onPageScroll(event) {}, */
  // 页面处理函数--用户点击右上角分享
  /* onShareAppMessage(options) {}, */
};
</script>

<style lang="scss" scoped>
.pageBox {
  display: flex;
  width: 100%;
  height: 100%;
  // background-color: #c7c7c7;

  
  .contentBox {
    position: absolute;
    top: 319rpx;
    background-color: white;
    height: 1570rpx;
    width: 100%;
    z-index: 10;
    border-radius: 57rpx;
    .insideBox {
      display: flex;
      flex-direction: column;
      .grey {
        width: 100%;
        height: 29rpx;
        background-color: #f5f5f5;
      }
      
      .comment{
        width: 640rpx;
        height: 73rpx;
        margin: 44rpx 55rpx 0 55rpx;
        background-color: #f5f5f5;
      }
      .buttons{
        width: 331rpx;
        height: 94rpx;
        margin:89rpx 221rpx 60rpx 221rpx;
        background-color: #f7b733;
      }
    }
  }
}
</style>

