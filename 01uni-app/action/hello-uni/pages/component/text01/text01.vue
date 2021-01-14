<template>

	<view>
	  <text selectable='true'>来了老弟</text>
	  <view>
	    <!-- 显示连续空格的方式 -->
	    <view>
	      <text space='ensp'>来了  老弟</text>
	    </view>
	    <view>
	      <text space='emsp'>来了  老弟</text>
	    </view>
	    <view>
	      <text space='nbsp'>来了  老弟</text>
	    </view>
	  </view>
	  
	  <view>
	    <text>skyblue</text>
	  </view>
	  
	   <!-- 是否解码 -->
	    <text decode='true'>&nbsp; &lt; &gt; &amp; &apos; &ensp; &emsp;</text>
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

</style>
