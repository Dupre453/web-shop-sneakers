<script setup>

import HeadDrawer from "@/components/HeadDrawer.vue";
import CartItemList from "@/components/CartItemList.vue";
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">
    <HeadDrawer/>
    <CartItemList/>

    <div class="flex flex-col gap-4 mt-7">

      <div class="flex gap-2">
        <span>Итого:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>22300 ₽</b>
      </div>

      <div class="flex gap-2">
        <span>Налог 5%:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>500 ₽</b>
      </div>

      <button
          disabled=""
          class="bg-lime-500 mt-4 w-full rounded-xl py-3 text-white hover:bg-lime-700 transition-all disabled:bg-slate-400 cursor-pointer">Оформить заказ</button>
    </div>
  </div>
</template>



<style scoped>

</style>