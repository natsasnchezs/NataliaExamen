<template>
  <div class="mx-10 my-5">
      
  <div class="grid grid-cols-4 gap-5">
      <div v-for="p in products">
     <ProductCard :product="p" />
  </div>
  </div>

  </div>

</template>

<script setup>


// fetch products
const { data: products } = await useFetch("https://fakestoreapi.com/products")
</script>
