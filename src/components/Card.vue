<script setup>
defineProps({
  imageUrl: String,
  title: String,
  price: Number,
  isFaforite: Boolean,
  isAdded: Boolean,
  onClickAdded: Function,
  onClickFavorite: Function
})
</script>

<template>
  <div
    class="relative bg-white border border-slate-100 rounded-3xl p-8 cursor-pointer transition hover:-translate-y-2 hover:shadow-xl"
  >
    <img
      :src="!isFaforite ? '/like-1.svg' : 'like-2.svg'"
      alt="like"
      class="absolute top-8 left-8"
      @click="on"
    />
    <img :src="imageUrl" alt="sneaker" />
    <p class="mt-2">{{ title }}</p>

    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-slate-400">Цена:</span>
        <b> {{ price }} руб.</b>
      </div>
      <img @click="onClickAdded" :src="!isAdded ? '/plus.svg' : 'checked.svg'" alt="plus" />
    </div>
  </div>
</template>
