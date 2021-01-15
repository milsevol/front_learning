<template>
	<view>
		<view>
			<text>{{pageName}}</text>
		</view>
		<view>
			<view>{{ flag ? '我是真的':'我是假的' }}</view>
		</view>

		<view>{{1+1}}</view>
		<view>
			<image :src="img"></image>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				pageName: "页面",
				img: 'http://destiny001.gitee.io/image/monkey_02.jpg'
			}
		},
		methods: {

		}
	}
</script>

<style>

</style>
