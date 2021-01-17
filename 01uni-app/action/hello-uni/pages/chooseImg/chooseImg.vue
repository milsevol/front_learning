<template>
	<view>
		<button @click="chooseImg" type="primary">上传图片</button>
		<view>
			<image v-for="item in imgArr" @click="previewImg(item)" :src="item" :key="index"></image>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				imgArr: []
			}
		},
		methods: {
			chooseImg() {
				uni.chooseImage({
					count: 9,
					success: res => {
						this.imgArr = res.tempFilePaths
					}
				})
			},
			previewImg (current) {
			  uni.previewImage({
			    urls: this.imgArr,
			    current
			  })
			}
		}
	}
</script>

<style>

</style>
