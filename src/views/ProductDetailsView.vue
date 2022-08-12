<script setup lang="ts">
import { useRoute } from "vue-router";
import json from "../assets/products.json";
import type { Product } from "@/models/Product";

const products: Product[] = json;
const route = useRoute();
const product: Product | undefined = products.find(
  productEntry => productEntry.id === parseInt(route.params.id[0])
);
console.log(route.params)
</script>

<template>
  <div>
    <h1>{{ product.title }}</h1>
    <h3>{{ product.brand }}</h3>
    <div>{{ product.price }}</div>
  </div>
</template>

<style lang="scss" scoped>

</style>