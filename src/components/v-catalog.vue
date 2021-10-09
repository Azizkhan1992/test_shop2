<template>
<div class = "v-catalog">
	<h3>Catalog</h3>
		<div class = "v-catalog_list">
		<vCatalogItem v-for = "product in products" :key = "product.article" :product_data = "product"></vCatalogItem>
		</div>
	
</div>
</template>

<script>

import vCatalogItem from './v-catalog-item';

export default{
	name: "v-catalog",
	components: {
	vCatalogItem
	},
	data(){
	return{
		 products: [
    {
     	image : "1.jpg",
      	name : "T-shirt 1",
      	price : 100,
      	article : "T1",
      	available : true
    },
    {
      	image : "2.jpg",
      	name : "T-shirt 2",
      	price : 150,
      	article : "T2",
      	available : true
    },
    {
      	image : "3.jpg",
      	name : "T-shirt 3",
      	price : 200,
      	article : "T3", 
      	available : true
    }
  ]
	}
	}
	
}
</script>

<style>
.v-catalog_list{
	display: flex;
	flex-wrap: wrap;
	justify-content: space-between;
	align-items: center;
}

</style>