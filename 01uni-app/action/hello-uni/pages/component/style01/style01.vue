<template>
	<view>
		<view>
			<text style="color: #4CD964;">哈哈</text>
		</view>
		<view>
			<text class="normal_view">内联样式</text>
		</view>
		<view>
			<text class="out_class">外联样式</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		methods: {

		}
	}
</script>

<style>
	@import "../../../common/css/test.css";

	.normal_view {
		color: #e91e63;
		font-size: x-large;
	}
</style>
