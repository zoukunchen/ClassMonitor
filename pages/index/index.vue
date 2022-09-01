<template>
	<view class="avatarItem">
		<image src="../../static/logo.png" class="avatarItem--1"></image>
		<text class="username">{{username}}</text>
		<view class="newbtn">
			<navigator url="/pages/lesson/lesson_add"><button class="addNew" type="primary" size="mini">新增</button></navigator>
		</view>
	</view>
	
</template>

<script>
export default {
	data() {
		return {
			username: '老·邹'
		};
	},
	methods: {}
};
</script>

<style>
	.avatarItem{
		display: flex;
		flex-wrap: nowrap;
		justify-content: space-between;
	}
	.avatarItem--1{
		height: 100rpx;
		width: 100rpx;
		margin-top: 50rpx;
		display: flex;
		margin-bottom: 50rpx;
		margin-left: 20rpx;
	}
	.username{
		font-size: 30rpx;
		color: #9e9e9e;
		font-family: sans-serif;
		font-weight: bold;
		margin-left: 10px;
		margin-right: 10px;
		margin-top: 30px;
		margin-bottom: 10px;
	}
	.addNew{
		margin-left: 10px;
		margin-right: 10px;
		margin-top: 70rpx;
		background-color: #3db86d;
		display: flex;
	
	}
	.newbtn{
		
	}
</style>
