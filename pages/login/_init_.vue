
<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{ title }}</text>
		</view>
	</view>
<!--这是一个<view>套<navigator>套<button>的组件。-->
	<view>
		<navigator url="/pages/login/login"><button class="priButton" type="primary">登录</button></navigator>
	</view>
</template>

<script>
export default {
	data() {
		return {
			title: 'To take a leap of faith.'
		};
	},
	onLoad() {},
	methods: {}
};
</script>

<style>
.content {
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
}

.logo {
	height: 400rpx;
	width: 400rpx;
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
	font-size: 40rpx;
	color: #9e9e9e;
	font-family: 'Times New Roman', Times, serif;
	font-style: italic;
}
.priButton {
	max-width: 200px;
	min-width: 150px;
	margin-top: 80px;
	background-color: #3db86d;
}
</style>
