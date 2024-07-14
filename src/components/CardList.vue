<script setup>
import Card from './Card.vue'
const onClickAdd = () => {
  alert('52!')
}
</script>
<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      title="Nike Blazer Mid Suede"
      imgeUrl="/sneakers/sneakers-1.jpg"
      :price="5000"
      :isFavorite="false"
      :onClickAdd="onClickAdd"
    />
  </div>
</template>
