<template>
  <h1>Product</h1>
  <ProductList :products="products" />
</template>
<script>
// import { products } from "../temp-data";
import ProductList from "../components/ProductList.vue";
import axios from "axios";

export default {
  name: "ProductPage",
  components: { ProductList },
  data() {
    return {
      products: [],
    };
  },
  async created() {
    const response = await axios.get("/api/products");
    const products = response.data;
    this.products = products;
  },
};
</script>
