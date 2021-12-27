<template>
	<view class="sport-remind-container">
		<view class="remind-box">
			<text class="remind-txt">运动提醒</text>
			<view class="button-box">
				<view class="button"></view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		name:"sport-remind",
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss" scoped>
.sport-remind-container{
	.remind-box{
		width: 700rpx;
		height: 100rpx;
		padding-left: 45rpx;
		background-color: white;
		border-radius: 26rpx;
		margin: 65rpx 25rpx;
		box-sizing: border-box;
		line-height: 100rpx;
		position: relative;
		.remind-txt{
			font-size: 36rpx;
		}
		.button-box{
			width: 84rpx;
			height: 42rpx;
			position: absolute;
			top: 30rpx;
			right: 27rpx;
			background-color: #F7B733;
			border-radius: 21rpx;
			.button{
				width: 34rpx;
				height: 34rpx;
				position: absolute;
				border-radius: 50%;
				right: 2px;
				top: 2px;
				background-color: white;
			}
		}

	}
}
</style>
