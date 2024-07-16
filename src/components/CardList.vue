<script setup>
import Card from './Card.vue'

const onClik = () => {
  alert('Added in favorite!')
}
</script>

<template>
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
  </div>
</template>
