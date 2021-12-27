<template>
  <view class="mine-container">
    <user-profile></user-profile>
    <user-info></user-info>
    <sport-remind></sport-remind>
  </view>
</template>

<script>
import SportRemind from "../../components/sport-remind/sport-remind.vue";
import userProfile from "../../components/user-profile/user-profile.vue";
export default {
  components: { userProfile, SportRemind },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.mine-container{
	width: 750rpx;
  height: 1500rpx;
	background-color: #f5f5f5;
}
</style>
