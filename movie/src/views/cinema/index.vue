<template>
	<div id="main">
		<div id="content">
		<Header title="附近影院"/>
			<div class="cinema_menu">
				<div class="city_switch">
					全城 <i class="iconfont icon-lower-triangle"></i>
				</div>
				<div class="brand_swtich">
					品牌 <i class="iconfont icon-lower-triangle"></i>
				</div>
				<div class="feature_switch">
					特色 <i class="iconfont icon-lower-triangle"></i>
				</div>
			</div>
			<Cilist />
		<Tabbar/>
		</div>
	</div>
</template>

<script type="text/javascript">
import Header from'@/components/Header/index.vue';
import Tabbar from'@/components/Tabbar/index.vue';
import Cilist from'@/components/Cilist/index.vue';

export default{
		name:'cinema',
		components:{
			Header,
			Tabbar,
			Cilist,

			
		},
		watch:{
			'$route'(cinema,movie){
				console.log(cinema);
				console.log(movie);
				

			}
		}

	}

</script>

<style scoped>
#content .cinema_menu{ width: 100%; height: 45px; border-bottom:1px solid #e6e6e6; display: flex; justify-content:space-around; align-items:center; background:white;}



</style>