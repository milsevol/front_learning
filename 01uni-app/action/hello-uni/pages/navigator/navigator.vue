<template>
	<view>
		<navigator url="/pages/about/about" hover-class="navigator-hover">
		  <button type="default">跳转到关于页面</button>
		</navigator>
		<navigator url="/pages/message/message" open-type="switchTab">
		  <button type="default">跳转到message页面</button>
		</navigator>
		<button type="primary" @click="goAbout">跳转到关于页面</button>
		<button type="primary" @click="goMessage">跳转到message页面</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			goAbout () {
			  uni.navigateTo({
			    url: '/pages/about/about',
			  })
			},
			goMessage () {
			  uni.switchTab({
			    url: '/pages/message/message'
			  })
			}
		}
	}
</script>

<style>

</style>
