<template>
  <div class="mx-10">

<ProductDetail :product="product" />

 </div>
</template>

<script setup>
const { id } = useRoute().params

const uri = 'https://fakestoreapi.com/products/' + id

// fetch the product
const { data: product } = await useFetch(uri)
  



</script>
