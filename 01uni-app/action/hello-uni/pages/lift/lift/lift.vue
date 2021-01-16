<template>
	<view>
		<view>生命周期</view>
		<view>
			<button type="primary" @click="startPull">开启下拉刷新</button>
			杭州学科
			<view v-for="(item,index) in arr" :key="index">
				{{item}}
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				arr: ['前端', 'java', 'ui', '大数据']
			}
		},
		methods: {

			startPull() {
				uni.startPullDownRefresh()
			},

			onLoad() {
				console.log('页面加载')
			},
			onShow() {
				console.log('页面显示')
			},
			onReady() {
				console.log('页面初次显示')
			},
			onHide() {
				console.log('页面隐藏')
			},
			onUnload() {
				console.log('页面卸载')
			},
			onBackPress() {
				console.log('页面返回...')
			},
			onShareAppMessage() {
				console.log('分享!')
			},
			onReachBottom() {
				console.log('下拉加载...')
			},
			onPageScroll() {
				console.log('页面滚动...')
			},

		},
		onPullDownRefresh() {
			this.arr = []
			setTimeout(() => {
				this.arr = ['前端', 'java', 'ui', '大数据']
				uni.stopPullDownRefresh()
			}, 1000);
			console.log('触发下拉刷新了')
		}
	}
</script>

<style>

</style>
