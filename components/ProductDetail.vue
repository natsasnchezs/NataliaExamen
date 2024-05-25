<template>
    <div class="card">
        <div class="grid grid-cols-2 gap-10">
        <div class="p-7">
            <img :src="product.image" class="mx-auto my-7">
        </div>
        <div class="p-7">
            <h2 class="text-4xl my-7">{{ product.title }}</h2>
            <p class="text-xl my-7">Precio - {{ product.price }} €</p>
            <h3 class="font-bold border-b-2 mb-4 pb-2">Descripción</h3>
            <p class="mb-7">{{ product.description }}</p>
            
            <!-- boton carrito compra -->
           <div class="flex gap-2">
            
            <div class="btn flex gap-2 px-3 py-2">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 3h1.386c.51 0 .955.343 1.087.835l.383 1.437M7.5 14.25a3 3 0 0 0-3 3h15.75m-12.75-3h11.218c1.121-2.3 2.1-4.684 2.924-7.138a60.114 60.114 0 0 0-16.536-1.84M7.5 14.25 5.106 5.272M6 20.25a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Zm12.75 0a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Z" />
</svg>
            <button>Cart </button>
            </div>
            
           </div>
           
        </div>
        </div>

    </div>
</template>

<script setup>
const { product } = defineProps(["product"])
</script>

<style scoped>
img {
    max-width: 400px;
}
</style>