<script setup lang="ts">
import type { Product } from "@/models/Product";

defineProps<{
  product: Product;
}>();
</script>

<template>
  <div class="card">
    <RouterLink :to="{ name: 'productRoute', params: { id: product.id } }">
      <img :src="product.thumbnail" class="card-img-top" alt="<product image" />
      <div class="card-body">
        <h5 class="card-title">{{ product.title }}</h5>
        {{ product.brand }}
      </div>
    </RouterLink>
  </div>
</template>

<style lang="scss" scoped>

</style>