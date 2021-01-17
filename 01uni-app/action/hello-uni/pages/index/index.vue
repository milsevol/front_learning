<template>
	<view class="content">
		<button type="primary" @click="gotoPage('/pages/component/text01/text01')">组件的基本使用</button>
		<button type="primary" @click="gotoPage('/pages/component/button01/button01')">按钮的用法</button>
		<button type="primary" @click="gotoPage('/pages/component/image01/image01')">图片</button>
		<button type="primary" @click="gotoPage('/pages/component/style01/style01')">样式</button>
		<button type="primary" @click="gotoPage('/pages/data/data01/data01')">数据绑定</button>
		<button type="primary" @click="gotoPage('/pages/event/event01/event01')">事件绑定</button>
		<button type="primary" @click="gotoPage('/pages/lift/lift/lift')">uni的生命周期</button>
		<button type="primary" @click="gotoPage('/pages/up/pull/pull')">上拉加载</button>
		<button type="primary" @click="gotoPage('/pages/get/sendGet/sendGet')">发送get请求</button>
		<button type="primary" @click="gotoPage('/pages/storage/storage')">数据缓存</button>
		<button type="primary" @click="gotoPage('/pages/chooseImg/chooseImg')">上传图片</button>
		<button type="primary" @click="gotoPage('/pages/navigator/navigator')">导航跳转</button>
		<button type="primary" @click="gotoPage('/pages/mycomponents/test/test')">自定义组件</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {
			gotoPage(page){
				 uni.navigateTo({
				    url: page,
				  })
			}
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
