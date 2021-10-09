<template>
<div class = "v-catalog-item">
	<img :src= "require('../assets/images/' + product_data.image)">
	<p class= "v-catalog-item_name">{{ product_data.name }}</p>
	<p class= "v-catalog-item_price">Price: {{ product_data.price }}</p>
	<button class = "v-catalog-item_add_to_cart_btn btn">Add to Cart</button>
</div>
</template>

<script>

export default{
	name: "v-catalog-item",
	data(){
	return{}
	},
	props:{
		product_data:{
		type: Object,
		default(){
		return{}
		}
		}
	}
}
</script>

<style>
.v-catalog-item{
	flex-basis: 25%;
	box-shadow: 0 0 8px 0;
	padding: 15px;
	margin: 10px;
}
</style>