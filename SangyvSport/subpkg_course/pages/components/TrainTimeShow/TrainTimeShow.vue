<template>
        <view class="timeShowBox">
          <text class="trainName">八段锦\n</text>
          <text class="trainShow">用时</text>
          <text class="trainTime">12</text>
          <text class="trainShow">分钟 </text>
        </view>
</template>

<script>
	export default {
		name:"TrainTimeShow",
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
      .timeShowBox {
        width: 100%;
        height: 232rpx;
        padding-top: 38rpx;
        text-align: center;
        line-height: 100rpx;
        .trainName {
          font-size: 48rpx;
          font-weight: 960;
        }
        .trainShow {
          font-size: 36rpx;
          font-weight: 545;
        }
        .trainTime {
          font-size: 80rpx;
          font-weight: 960;
          color: #f7b733;
        }
      }
</style>
