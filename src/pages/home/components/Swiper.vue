<template>
	<div class="wrapper">
		<swiper :options="swiperOption">
		    <!-- slides -->
		    <swiper-slide v-for='item of swiperList' :key='item.id'>
		    	<img class="swiper-img" :src="item.imgUrl" />
		    </swiper-slide>
		    
		    <!-- Optional controls -->
		    <div class="swiper-pagination"  slot="pagination"></div>
		   
	 	</swiper>
	</div>
</template>

<script>
	export default {
		name : 'HomeSwiper',
		data () {
			return {
				swiperOption : {
					pagination : '.swiper-pagination',
					loop : true
				},
				swiperList : [{
					id : '001',
					imgUrl : '../../assets/images/cookbook-img01.jpg'
					},{
					id : '002',
					imgUrl : 'https://gss0.bdstatic.com/5bVWsj_p_tVS5dKfpU_Y_D3/res/r/image/2017-09-26/352f1d243122cf52462a2e6cdcb5ed6d.png'
					},{
					id : '003',
					imgUrl : 'https://gss0.bdstatic.com/5bVWsj_p_tVS5dKfpU_Y_D3/res/r/image/2017-09-27/297f5edb1e984613083a2d3cc0c5bb36.png'
					}]
			}
		}
	}
</script>

<style scoped>
	.wrapper >>> .swiper-pagination-bullet-active { background: #ff6d00;}
	.wrapper{ overflow:hidden; width:100%; height: 18px; padding-bottom: 31.25%;}
	.swiper-img{ width:100%}
</style>