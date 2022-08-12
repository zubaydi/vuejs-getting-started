<script setup lang="ts">
import type { Product } from "@/models/Product";

const props = defineProps<{
  product: Product;

}>();
</script>

<template>
{{product.title}}
{{product.brand}}
{{product.thumbnail}}
 
</template>

<style lang="scss" scoped>

</style>