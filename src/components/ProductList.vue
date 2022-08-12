<script setup lang="ts">
import type { Product } from "@/models/Product";
import ProductComponent from "./productComponent.vue";

const props = defineProps<{
  products: Product[];
}>();
</script>

<template>
  <h1>Products</h1>

  <div class="container grid">
    <div class="col" v-for="product in props.products" :key="product.id">
      <div class="card">
      <ProductComponent :product="product"></ProductComponent>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>

</style>