<script setup>
import Card from './Card.vue'

defineProps({
  items: Array
})

const onClickAdd = () => {
  alert('52!')
}
</script>
<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      v-for="item in items"
      :key="item.id"
      :title="item.title"
      :imgeUrl="item.imageUrl"
      :price="item.price"
      :onClickAdd="onClickAdd"
    />
  </div>
</template>
