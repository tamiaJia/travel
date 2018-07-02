<template>
	<div>
		<div class="recommend-title">热销推荐</div>	
		<ul>
			<li class="item border-bottom" v-for="item of recommendList" :key="item.id">
			 	<img class="item-img" :src="item.imgUrl" alt="" />
				<div class="item-info">
					<p class="item-title">{{item.title}}</p>
					<p class="item-desc">{{item.desc}}</p>
					<button class="item-button">查看详情</button>
				</div>
			</li>
		</ul>
	</div>
</template>
<script>
	export default{
		name:'HomeRecommend',
		data () {
			return{
				recommendList:[
					{
						id:'0001',
						imgUrl:'http://img1.qunarzz.com/sight/p0/1803/9d/9d862d8166170089a3.img.jpg_200x200_8974965b.jpg',
						title:'北京园博园',
						desc:'繁花似锦的夏天正迎面而来，夏天是美好的，夏天是多姿多彩的，夏天的北京园博园绿意正浓、水韵灵动、色彩斑斓、美景如画，值得去探寻！'
					},
					{
						id:'0002',
						imgUrl:'http://img1.qunarzz.com/sight/p0/1803/9d/9d862d8166170089a3.img.jpg_200x200_8974965b.jpg',
						title:'北京园博园',
						desc:'繁花似锦的夏天正迎面而来，夏天是美好的，夏天是多姿多彩的，夏天的北京园博园绿意正浓、水韵灵动、色彩斑斓、美景如画，值得去探寻！'
					},
					{
						id:'0003',
						imgUrl:'http://img1.qunarzz.com/sight/p0/1803/9d/9d862d8166170089a3.img.jpg_200x200_8974965b.jpg',
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
	.recommend-title
		margin-top: .2rem
		line-height: .8rem
		background: #eee
		text-indent: .2rem
	.item
		height: 1.9rem
		display: flex
		
		.item-img
			width 1.7rem
			height: 1.7rem
			padding: .1rem
		.item-info
			flex: 1 
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
			.item-button
				background: #ff9300
				padding: 0 .2rem
				border-radius: .06rem
				margin-top: .16rem
				color: #fff
				line-height: .44rem
</style>