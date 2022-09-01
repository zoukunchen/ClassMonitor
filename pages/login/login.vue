<template>
	<view>
	<view class="content">
		<image class="logo_sml" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
	</view>
	</view>
	<view>
			<view>
				<form @submit="formSubmit">
					<view class="uni-form-item uni-column">
						<view class="intro_text">昵称</view>
						<input class="uni-input_sml" name="input" placeholder="大家都会看到这个名字" />
					</view>
					<view class="uni-form-item uni-column">
						<view class="intro_text">个人简介</view>
						<input class="uni-input_lg" name="input" placeholder="简单介绍自己" />
					</view>
					<view class="uni-form-item uni-column">
						<view class="intro_text">注册码</view>
						<input class="uni-input_sml" name="input" placeholder="注册码仅能使用一次" />
					</view>
					<view>
						<button form-type="submit" class="priButton" type="primary">登录</button>
					</view>
				</form>
			</view>
	</view>
	
</template>

<script>
	export default {
		data() {
			return {
				title: 'To take a leap of faith.'
			}
		},
		onLoad() {
	
		},
		methods: {
	
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

	.logo_sml {
		height: 100rpx;
		width: 100rpx;
		margin-top: 50rpx;
		display: flex;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 30rpx;
		color: #9e9e9e;
		font-family: 'Times New Roman', Times, serif;
		font-style: italic;
	}
	.priButton{
		max-width: 200px;
		min-width: 150px;
		margin-top: 50px;
		background-color: #3DB86D;
	}
		.uni-form-item .title {
		padding: 20rpx 0;
	}
	.intro_text{
		font-size: 30rpx;
		color: #9e9e9e;
		font-family: sans-serif;
		font-weight: bold;
		margin-left: 40px;
		margin-right: 40px;
		margin-top: 30px;
		margin-bottom: 10px;
		
	}
	.uni-input_sml{
		margin-left: 30px;
		margin-right: 30px;
		background-color: #eeeeee;
		padding: 10px;
		font-size: 10pt;
		border-radius: 8px;
	}
	.uni-input_lg{
		margin-left: 30px;
		margin-right: 30px;
		background-color: #eeeeee;
		padding: 10px;
		padding-bottom: 100px;
		font-size: 10pt;
		border-radius: 8px;
	}
</style>
