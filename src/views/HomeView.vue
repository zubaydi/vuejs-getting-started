<script setup lang="ts">
import ProductList from "../components/ProductList.vue";
import json from "../assets/products.json";
import type { Product } from "@/models/Product";
import SearchBarComponent from "../components/SearchBarComponent.vue";

const products: Product[] = json;
//const search = "" : string ; 
</script>

<template>
  <div class="home">
    <!--SearchBarComponent @emit-execute-search="search"></SearchBarComponent-->
    <ProductList :products="products"></ProductList>
  </div>
</template>

<style scoped lang="scss"></style>
