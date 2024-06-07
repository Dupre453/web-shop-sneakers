<script setup>
import Card from "@/components/Card.vue";


const onClickAdd = () => {
  alert('Добавить')
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
        :isFavorite="true"
        :is-added="true"
        :price="5000"
        imageUrl="./src/assets/sneakers/sneakers-1.jpg"
        title="Мужские Кроссовки Nike Blazer Mid Suede"
        :onClickAdd="onClickAdd"
    />
    <Card/>
    <Card/>
  </div>
</template>



<style scoped>

</style>