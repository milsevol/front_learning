<template>
	<view>
		<button @click="sendGet">发送请求</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		methods: {
			sendGet() {
				uni.request({
					url: 'http://localhost:8082/api/getlunbo',
					success(res) {
						console.log(res)
					}
				})
			}
		}
	}
</script>

<style>

</style>
