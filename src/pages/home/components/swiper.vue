<template>
	<div class="wrapper">
	 	<swiper :options="swiperOption">
    <!-- slides -->
	    <swiper-slide v-for="item of swiperList" :key="item.id">
	    	<img class="swiper-img" :src="item.imgUrl"/>
	    </swiper-slide>
	    <!-- Optional controls -->
	    <div class="swiper-pagination"  slot="pagination"></div>
  	</swiper>
	</div>
</template>
<script type="text/javascript">
	
export default{
	name:'HomeHeader',
	data() {
		return{
			swiperOption:{
				pagination:'.swiper-pagination',
				loop:true
			},
			swiperList:[
				{
					id:'001',
					imgUrl:'http://img1.qunarzz.com/piao/fusion/1706/b9/6b91b49794f46402.jpg_750x200_d7f254e2.jpg'
				},
				{
					id:'002',
					imgUrl:'http://img1.qunarzz.com/piao/fusion/1809/c6/2467595fffc3b302.jpg_750x200_cca13d51.jpg'
				}
			]
		}
  }
}
</script>

<style lang="stylus" scoped>
	.wrapper >>> .swiper-pagination-bullet-active
		background:#fff
	.swiper-img
		width:100%
</style>