<script setup lang="ts">

import type {Product} from '../models/Product';
import {useRoute} from 'vue-router';

const route = useRoute();
</script>

<template>
  <div>
    {{ route.params.id }}
  </div>
</template>

<style scoped>

</style>