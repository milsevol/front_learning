<template>
	<view>
		<button type="primary" @click="setStor1">存储数据 (异步)</button>
		<button type="primary" @click="setStor2">存储数据（同步)</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		methods: {
			setStor1() {
				uni.setStorage({
					key: 'id',
					data: 100,
					success() {
						console.log('存储成功')
					}
				})
			},
			setStor2() {
				uni.setStorageSync('id2',100)
			}
		}
	}
</script>

<style>

</style>
