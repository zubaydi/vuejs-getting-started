<script setup lang="ts">
import ProductList from "../components/ProductList.vue";
import json from "../assets/products.json";
import type { Product } from "@/models/Product";

const products: Product[] = json;
</script>

<template>
  <div class="home">
    <ProductList :products="products"></ProductList>
  </div>
</template>

<style scoped lang="scss"></style>
