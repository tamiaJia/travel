<template>
	<div class="wrapper">
		<swiper :options="swiperOption">
	    <!-- slides -->
	    <swiper-slide v-for='item of swiperList' :key='item.id'>
	    	<img class="swiper-img" :src="item.imgUrl" alt="">
	    </swiper-slide>
	    <!-- Optional controls -->
	    <div class="swiper-pagination"  slot="pagination"></div>
	  </swiper>
  </div>
</template>
<script>
export default{
	name: 'HomeSwiper',
	data () {
		return {
			swiperOption:{
				pagination:'.swiper-pagination',
				loop: true
			},
			swiperList:[
			 {
			 	id:'0001',
			 	imgUrl:'http://img1.qunarzz.com/piao/fusion/1804/bd/8e4a1c3f470d3702.jpg_750x200_f1f0a8c7.jpg'
			 },
			 {
			 	id:'0002',
			 	imgUrl:'http://img1.qunarzz.com/piao/fusion/1806/fc/e47aa3e1c67bbc02.jpg_750x200_0f3eecf8.jpg'
			 }
			]
		}
	}
}
</script>
<style lang="stylus" scoped>
.wrapper>>>.swiper-pagination-bullet-active
	background-color: #fff
.wrapper
	overflow: hidden
	width: 100%
	height: 0
	padding-bottom: 26.666667%
	background: #ccc
	.swiper-img
		width: 100%
</style>