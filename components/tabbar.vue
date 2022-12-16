<template>
	<view>
		<view class="u-page">
			<!-- 所有内容的容器 -->
		</view>
		<!-- 与包裹页面所有内容的元素u-page同级，且在它的下方 -->
		<u-tabbar v-model="current" :list="list" :mid-button="true" active-color='#5098FF'></u-tabbar>
	</view>
</template>

<script>
	export default {
		name:"tabbar",
		data() {
			return {
				list: [{
						iconPath: "home",
						selectedIconPath: "home-fill",
						text: '首页',
						isDot: true,
						customIcon: false,
						pagePath: '/pages/tabbar/tabbar1',
					},
					{
						iconPath: "photo",
						selectedIconPath: "photo-fill",
						text: '项目汇总',
						customIcon: false,
						pagePath: '/pages/tabbar/tabbar2',
					},
					{
						iconPath: "https://cdn.uviewui.com/uview/common/min_button.png",
						selectedIconPath: "https://cdn.uviewui.com/uview/common/min_button_select.png",
						text: '发起项目',
						midButton: true,
						customIcon: false,
						pagePath: '/pages/tabbar/tabbar3',
					},
					{
						iconPath: "play-right",
						selectedIconPath: "play-right-fill",
						text: '医疗咨询',
						customIcon: false,
						pagePath: '/pages/tabbar/tabbar4',
					},
					{
						iconPath: "account",
						selectedIconPath: "account-fill",
						text: '我的',
						// count: 23,
						isDot: false,
						customIcon: false,
						pagePath: '/pages/tabbar/tabbar5',
					}
				],
				current: 0
			}
		},
	}
</script>

<style>

</style>