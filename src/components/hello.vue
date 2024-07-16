<script setup>
defineProps({
  title: String,
  price: Number
})
</script>

<template>
  <div class="products">
    <h2>Товар: {{ title }}</h2>
    <h3>Цена: {{ price }}</h3>
    <slot class="color"></slot>
  </div>
</template>

<style scoped>
.products {
  border: 1px solid blue;
  padding: 10px;
  margin-bottom: 10px;
}
</style>
