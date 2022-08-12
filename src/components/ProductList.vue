<script setup lang="ts">
import type { Product } from "@/models/Product";
import ProductComponent from "./ProductComponent.vue";

defineProps<{
  products: Product[];
}>();
</script>

<template>
  <h1>Products</h1>
  <div class="container grid">
    <div class="col" v-for="product in products" :key="product.id">
      <ProductComponent :product="product" class="product"></ProductComponent>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.product {
  width: 100px;
}
</style>
