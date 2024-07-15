<script setup>
import DrawerHead from './DrawerHead.vue'
import CartitemList from './CartitemList.vue'
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 h-full fixed right-9 top-0 z-20 p-8">
    <DrawerHead />

    <CartitemList />

    <div class="flex flex-col gap-3 mt-7">
      <div class="flex gap-2">
        <span>Загалом:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>12990 ₴</b>
      </div>

      <div class="flex gap-2">
        <span>Податок 5%</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>650 ₴</b>
      </div>
      <button 
    disabled=""
    class="mt-3 disabled:bg-slate-300 bg-orange-300 w-full rounded-3xl py-3 text-white hover:bg-orange-400 active:bg-orange-500 cursor-pointer">
    Оформити замовнення</button>
    </div>
    
  </div>
</template>
