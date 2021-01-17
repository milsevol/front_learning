<template>
	<view>
		<login :msg="msg" @myEvent="getMsg"></login>

	</view>
</template>

<script>
	import login from "@/components/login/login.vue"
	export default {
		data() {
			return {
				msg: 'hello'
			}
		},
		components: {
			login
		},
		methods: {
			getMsg(res) {
				console.log(res)
			}
		}
	}
</script>

<style>

</style>
