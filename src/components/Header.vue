<template>
  <header class="flex justify-between border-b border-slate-200 px-10 py-8">

    <div class="flex items-center gap-4">
      <img src="../assets/logo%20(1).png" alt="Logo" class="w-10">
      <div>
        <h2 class="text-xl font-bold uppercase">Vue Sneakers</h2>
        <p class="text-slate-400">Магазин лучших кроссовок</p>
      </div>
    </div>

    <ul class="flex items-center gap-10">
      <li class="flex items-center gap-3 text-slate-500 cursor-pointer hover:text-black transition-all">
        <img src="../assets/cart.svg" alt="Cart">
        <b>1250 руб.</b>
      </li>

      <li class="flex items-center gap-3 text-slate-500 cursor-pointer hover:text-black transition-all">
        <img src="../assets/heart.svg" alt="Cart">
        <span>Закладки</span>
      </li>

      <li class="flex items-center gap-3 text-slate-500 cursor-pointer hover:text-black transition-all">
        <img src="../assets/profile.svg" alt="Cart">
        <span>Профиль</span>
      </li>
    </ul>


  </header>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>

</style>