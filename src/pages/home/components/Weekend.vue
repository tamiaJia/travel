<template>
	<div>
		<div class="weekend-title">周末去哪儿</div>	
		<ul>
			<li class="item border-bottom" v-for="item of recommendList" :key="item.id">
				<div class="item-img-wrapper">
			 		<img class="item-img" :src="item.imgUrl" alt="" />
				</div>
				<div class="item-info">
					<p class="item-title">{{item.title}}</p>
					<p class="item-desc">{{item.desc}}</p>
				</div>
			</li>
		</ul>
	</div>
</template>
<script>
	export default{
		name:'HomeWeekend',
		data () {
			return{
				recommendList:[
					{
						id:'0001',
						imgUrl:'http://img1.qunarzz.com/sight/source/1505/aa/7baaf8a851d221.jpg_r_640x214_1431200f.jpg',
						title:'北京园博园',
						desc:'繁花似锦的夏天正迎面而来，夏天是美好的，夏天是多姿多彩的，夏天的北京园博园绿意正浓、水韵灵动、色彩斑斓、美景如画，值得去探寻！'
					},
					{
						id:'0002',
						imgUrl:'http://img1.qunarzz.com/sight/source/1505/9e/21df651e19af5d.jpg_r_640x214_3ea5bb38.jpg',
						title:'北京园博园',
						desc:'繁花似锦的夏天正迎面而来，夏天是美好的，夏天是多姿多彩的，夏天的北京园博园绿意正浓、水韵灵动、色彩斑斓、美景如画，值得去探寻！'
					},
					{
						id:'0003',
						imgUrl:'http://img1.qunarzz.com/sight/source/1505/ce/bc89bc2f0e33ea.jpg_r_640x214_3e408453.jpg',
						title:'北京园博园',
						desc:'繁花似锦的夏天正迎面而来，夏天是美好的，夏天是多姿多彩的，夏天的北京园博园绿意正浓、水韵灵动、色彩斑斓、美景如画，值得去探寻！'
					}
				]
			}
		}
	}
</script>
<style lang="stylus" scoped>
@import '~styles/mixins.styl'
	.weekend-title
		margin-top: .2rem
		line-height: .8rem
		background: #eee
		text-indent: .2rem
	.item-img-wrapper
		overflow: hidden
		height: 0
		padding-bottom: 33.9%
		.item-img
			width: 100%
	.item-info
		padding: .1rem
		min-width:0
		.item-title
			line-height .54rem
			font-size: .32rem
			ellipsis()
		.item-desc	
			line-height: .4rem
			coloe: #ccc
			ellipsis()
</style>