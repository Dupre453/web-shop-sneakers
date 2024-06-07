<script setup>
defineProps({
  imageUrl: String,
  title: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClickAdd: Function,
  onClickFavorite: Function,
})
</script>

<template>
  <div class="relative bg-white border border-slate-100 rounded-3xl p-8 cursor-pointer hover:-translate-y-2 hover:shadow-xl">
    <img
        @click="onClickFavorite"
        :src="!isFavorite ? './src/assets/like-1.svg' : './src/assets/like-2.svg'"
        alt="like"
        class="absolute top-8 left-8"

    >
    <img :src="imageUrl" alt="sneakers">
    <p class="mt-2">{{title}}</p>
    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-slate-400">Цена:</span>
        <b>{{price}} руб.</b>
      </div>
      <img
          @click="onClickAdd"
          :src="!isAdded ? './src/assets/plus.svg' : './src/assets/checked.svg'"
          alt="plus"
      >
    </div>
  </div>
</template>



<style scoped>

</style>