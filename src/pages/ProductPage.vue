<template>
  <h1>Product</h1>
  <ProductList :products="products" />
</template>
<script setup>
import { products } from "../temp-data";
import ProductList from "../components/ProductList.vue";
// export default {
//   name: "ProductPage",
//   data() {
//     return {
//       products,
//     };
//   },
// };
</script>
