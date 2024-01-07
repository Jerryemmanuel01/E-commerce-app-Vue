<template>
  <h1>Product</h1>
  <div class="grid-wrap">
    <div class="product-item" v-for="product in products" :key="product.id">
      <img :src="product.imageName" alt="" />
      <h3 class="product-name">{{ product.name }}</h3>
      <p class="product-price">{{ product.price }}</p>
      <button>View Details</button>
    </div>
  </div>
</template>
<script setup>
import { products } from "../temp-data";
// export default {
//   name: "ProductPage",
//   data() {
//     return {
//       products,
//     };
//   },
// };
</script>
