<script setup>
import Card from './Card.vue'

const onClik = () => {
  alert('Added in favorite!')
}
</script>

<template>
  <div class="p-10">
    <h2 class="text-3xl font-bold mb-8">Все кроссовки</h2>
    <div class="grid grid-cols-4 gap-5">
      <Card
        imageUrl="/public/sneakers/sneakers-1.jpg"
        title="Мужские Кроссовки Nike Blazer Mid Suede"
        :price="12599"
        :onClickFavorite="onClik"
      />
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
    </div>
  </div>
</template>
