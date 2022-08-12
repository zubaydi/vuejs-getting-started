<script setup lang="ts">
import type { Product } from "@/models/Product";

const props = defineProps<{
  products: Product[];
}>();
</script>

<template>
  <h1>Products</h1>

  <div class="container grid">
    <div class="col" v-for="product in props.products" :key="product.id">
      <div class="card">
        {{ product.title }}
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>

</style>