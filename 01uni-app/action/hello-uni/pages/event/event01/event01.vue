<template>
	<view>
		<button @click="tapHandle">点我啊</button>
		<button @click="tapHandle2(1,$event)">点我啊</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		methods: {
			tapHandle(e) {
				console.log(e)
			},
			tapHandle2(num, e) {
				console.log(num, e)
			}
		}
	}
</script>

<style>

</style>
