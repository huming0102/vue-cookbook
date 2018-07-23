<template>
	<div class="header">
		<div class="header-left">
			<span class="iconfont back-icon">&#xe679;</span>
		</div>
		<div class="header-input">
			<span class="iconfont">&#xe612;</span>
			搜菜谱、食材、相克等
		</div>
		<div class="header-right">
			城市
			<span class="iconfont arrow-icon">&#xe716;</span>
		</div>
	</div>
</template>

<script>
	export default {
		name : 'HomeHeader'
	}
</script>

<style scoped>
	/*@import '~@/assets/style/varibles.styl'*/
	.header{ display:flex;line-height:44px; background: #ff6d00; color: #fff;}
	.header .header-left{width:32px; float: left;text-align:right;}
	.header-left .back-icon{ font-size:20px}
	.header .header-input{flex:1; margin-top:6px; margin-left:10px; padding-left:10px; height: 32px; line-height: 32px; background: #fff; border-radius: 5px; color:#ccc }
	.header .header-right{width:62px; text-align: center; float: right;}
	.header-right .arrow-icon{font-size:22px; margin-left:-6px}
</style>