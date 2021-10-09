<template>
	<div class = "v-main-wrapper">
		<h1>{{ title }}</h1>
		<vCatalog></vCatalog>
		<vCart></vCart>
	</div>
</template>

<script>

import vCatalog from './v-catalog';
import vCart from './v-cart';

export default{
	name: 'v-main-wrapper',
	components:{
	vCatalog,
	vCart
	},
	data(){
	return{
	title: 'Assalom'
	}
	}
}
</script>

<style scoped>
	.v-main-wrapper{
		max-width: 900px;
		margin: 0 auto;
	}
</style>