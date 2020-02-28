<template>
	<div id="main">
		
		<Header title="我的"/>
		<div id="content">
			<Login />
		</div>

		<Tabbar/>
		
	</div>
</template>

<script type="text/javascript">
import Header from'@/components/Header/index.vue';
import Tabbar from'@/components/Tabbar/index.vue';
import Login from'@/components/Login/index.vue';

export default{
		name:'mine',
		components:{
			Header,
			Tabbar,
			Login

			
		}
}
</script>

<style>

</style>