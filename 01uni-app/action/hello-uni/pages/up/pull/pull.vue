<template>
	<view>
		<button type="primary" @click="startPull">开启下拉刷新</button>
		杭州学科
		<view v-for="(item,index) in arr" :key="index">
			{{item}}
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				arr: ['前端', 'java', 'ui', '大数据', '前端', 'java', 'ui', '大数据']
			}
		},
		onReachBottom() {
			console.log('触底了')
		}
	}
</script>

<style>
	view {
		height: 100px;
		line-height: 100px;
	}
</style>
