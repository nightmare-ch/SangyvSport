<template>
  <view class="trainFeeling-container">
    <text class="feeling">本次训练感受如何</text>
    <view class="trainFeeling" v-if="flag">
      <view class="standards">
        <view class="feeling-easy fB" @click="feelingShowEasy()">
          <image
            class="feelingImage"
            src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程完成/太简单了.png"
            mode="scaleToFill"
          />
          <text class="feelingText">太简单了</text>
        </view>
        <view class="feeling-good fB" @click="feelingShowGood()">
          <image
            class="feelingImage"
            src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程完成/太棒了.png"
            mode="scaleToFill"
          />
          <text class="feelingText">太棒了</text>
        </view>
        <view class="feeling-hard fB" @click="feelingShowHard()">
          <image
            class="feelingImage"
            src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程完成/太难了.png"
            mode="scaleToFill"
          />
          <text class="feelingText">太难了</text>
        </view>
      </view>
    </view>
    <view class="selected" v-if="flag1">
      <view class="view-selected">
        <image
          class="feelingImage"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程完成/easy-clicked.png"
          mode="scaleToFill"
        />
        <text class="feelingText">太棒了，可以挑战更高难度的运动！</text>
      </view>
    </view>
    <view class="selected" v-if="flag2">
      <view class="view-selected">
        <image
          class="feelingImage"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程完成/good-clicked.png"
          mode="scaleToFill"
        />
        <text class="feelingText">太棒了，继续坚持！</text>
      </view>
    </view>
    <view class="selected" v-show="flag3">
      <view class="view-selected">
        <image
          class="feelingImage"
          src="https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程完成/hard-clicked.png"
          mode="scaleToFill"
        />
        <text class="feelingText">别气馁，可以先选择难度较低的运动！</text>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  name: "TrainFeeling",
  data() {
    return {
      flag: true,
      flag1: false,
      flag2: false,
      flag3: false,
    };
  },
  methods: {
    setData: function (field, val) {
      this.$set(this.$data, field, val);
      //如果需要提交请求,下面这样是不行的,提交的是field字符串
      $.post("url", { field: val }, function () {});
      //需要这样
      var json = {};
      json[field] = value;
      $.post("url", json, function () {});
    },
    feelingShowEasy: function () {
      this.flag = !this.flag;
      this.flag1 = !this.flag1;
    },
    feelingShowGood: function () {
      this.flag = !this.flag;
      this.flag2 = !this.flag2;
    },
    feelingShowHard: function () {
      this.flag = !this.flag;
      this.flag3 = !this.flag3;
    },
  },
};
</script>

<style lang="scss">
.trainFeeling-container {
  margin-top: 26rpx;

  .feeling {
    font-size: 48rpx;
    font-weight: 550;
    margin-left: 56rpx;
  }

  .trainFeeling {
    height: 100%;
    width: 100%;
    margin-top: 26rpx;
    .standards {
      display: flex;
      margin: 26rpx 86rpx;
      justify-content: space-between;
      .fB {
        display: flex;
        flex-direction: column;
        align-items: center;
        .feelingImage {
          width: 106rpx;
          height: 106rpx;
        }
        .feelingText {
          margin-top: 19rpx;
          font-weight: 550;
        }
      }
    }
  }
  .view-selected {
    margin-top: 26rpx;
    display: flex;
    flex-direction: column;
    align-items: center;
    .feelingImage {
      width: 106rpx;
      height: 106rpx;
    }
    .feelingText {
      margin-top: 19rpx;
      font-weight: 550;
    }
  }
}
</style>
