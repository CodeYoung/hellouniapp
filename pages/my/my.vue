<template>
	<view>
		今天星期六
		<button @click="toindex">跳转回{{$data.name}}首页</button>
		<button @click="toindex">跳转回{{$data.name1}}首页</button>
		<button @click="toindex">跳转回{{$data.name2}}首页</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
			    name:"李杨",
				name1:"zy",
				name2:"pp"
			}
		},
		methods: {
			toindex()
			{
				uni.navigateTo({
					url:"/pages/index/index"
				})
				
			}
		}
	}
</script>

<style>

</style>
