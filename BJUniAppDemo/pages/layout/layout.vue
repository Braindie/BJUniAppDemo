<template>
	<view class="layout">
		<view v-for="(title, index) in list" class="layout-list" :key="index">
			<view class="layout-list-item" @click="clickItem">
				{{ title }}
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: ["nvue"]
			}
		},
		methods: {
			clickItem() {
				console.log("click");
				uni.navigateTo({
					url: '/pages/layout/nvuePage'
				})
			}
		}
	}
</script>

<style>

</style>
