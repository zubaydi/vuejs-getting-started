<script setup lang="ts">
import HelloWorld from "../components/HelloWorld.vue";
import ProductList from "../components/ProductList.vue";
import json from "../assets/products.json";
import type {Product} from '@/models/Product';

const products: Product[] = json;
</script>

<template>
  <div class="home">
    <HelloWorld first-name="Zachary" last-name="Snow" />
    <ProductList :products="products"></ProductList>
  </div>
</template>

<style scoped lang="scss"></style>
