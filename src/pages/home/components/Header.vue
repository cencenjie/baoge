<template>
	<div class="header">
		<div class="header-left">
			<div class="iconfont back-icon">&#xe601;</div>
		</div>
		<div class="header-input">
			<span class="iconfont ">&#xe637;</span>
			输入城市/景点/游玩主题
		</div>
		<div class="header-right">城市<span class="iconfont down-icon">&#xe62e;</span></div>
	</div>
</template>
<script type="text/javascript">
	
export default{
	name:'HomeHeader',
	}
</script>

<style lang="stylus" scoped>
	// @import '~@/assets/styles/varibles.styl'
		@import '~styles/varibles.styl'
	.header
		display:flex
		line-height:.86rem
		background-color:$bgColor
		color:#fff
		.header-left
			width:.64rem
			float:left
			.back-icon
				text-align:center
				font-size:.4rem			
		.header-input
			flex:1
			height:.64rem
			line-height:.64rem
			margin-top:.12rem
			margin-left:.2rem
			background-color:#fff
			border-radius:.1rem
			color:#aaa
			padding-left:.06rem
		.header-right
			width:1.24rem
			float:right
			text-align:center			
</style>