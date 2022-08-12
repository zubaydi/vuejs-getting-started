<script setup lang="ts">
import type { Product } from "../models/Product";
import { defineProps } from "vue";

const props = defineProps<{
  products: Product[];
}>();
</script>

<template>
  <h1>Product</h1>

  <div class="container grid">
    <div class="col" v-for="product in props.products" :key="product.id">

    </div>
  </div>
</template>



<style scoped>

</style>