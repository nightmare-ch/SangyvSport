<script>
	export default {
		onLaunch: function() {
			
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style lang="scss">
	/*每个页面公共css */
	@import "https://7463-tcb-urue3qthyxmtooj6f3e3b-e6aa21-1308556956.tcb.qcloud.la/课程完成/icon-comment/iconfont.css";
	@import '@/uni_modules/uni-scss';
	
	
	// 设置整个项目的背景色
	page {
		background-color: #f5f5f5;
	}

	
</style>
