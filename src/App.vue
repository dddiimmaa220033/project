<script setup>
import Header from './components/Header.vue'
import CardList from './components/CardList.vue'
import Drawer from './components/Drawer.vue'

const items = [
  [
    {
      id: 1,
      title: 'Nike Blazer Mid Suede',
      price: 12999,
      imageUrl: '/sneakers/sneakers-1.jpg'
    },
    {
      id: 2,
      title: ' Nike Air Max 270',
      price: 15600,
      imageUrl: '/sneakers/sneakers-2.jpg'
    },
    {
      id: 3,
      title: ' Nike Blazer Mid Suede',
      price: 8499,
      imageUrl: '/sneakers/sneakers-3.jpg'
    },
    {
      id: 4,
      title: ' Puma X Aka Boku Future Rider',
      price: 7800,
      imageUrl: '/sneakers/sneakers-4.jpg'
    },
    { id: 5, title: 'Future Rider', price: 9550, imageUrl: '/sneakers/sneakers-5.jpg' },
    { id: 6, title: 'Black Edition', price: 16999, imageUrl: '/sneakers/sneakers-6.jpg' },
    {
      id: 7,
      title: ' Orange Boomb Edition',
      price: 7499,
      imageUrl: '/sneakers/sneakers-7.jpg'
    },
    {
      id: 8,
      title: ' Nike Air Max 270',
      price: 15600,
      imageUrl: '/sneakers/sneakers-8.jpg'
    },
    {
      id: 9,
      title: ' Nike Air Force 1',
      price: 5900,
      imageUrl: '/sneakers/sneakers-9.jpg'
    },
    {
      id: 10,
      title: ' Adidas Ultraboost',
      price: 11500,
      imageUrl: '/sneakers/sneakers-10.jpg'
    },
    {
      id: 11,
      title: ' Puma Clyde All-Pro',
      price: 7600,
      imageUrl: '/sneakers/sneakers-11.jpg'
    },
    {
      id: 12,
      title: ' Converse Chuck Taylor All-Star',
      price: 13000,
      imageUrl: '/sneakers/sneakers-12.jpg'
    },
    { name: 'Root', email: 'admin@email.com', id: 13 },
    { id: 14 },
    {
      0: {
        id: 1,
        title: 'Nike Blazer Mid Suede',
        price: 12999,
        imageUrl: '/sneakers/sneakers-1.jpg',
        isFavorite: true,
        favoriteId: 3,
        isAdded: false
      },
      1: {
        id: 2,
        title: ' Nike Air Max 270',
        price: 15600,
        imageUrl: '/sneakers/sneakers-2.jpg',
        isFavorite: true,
        favoriteId: 1,
        isAdded: false
      },
      2: {
        id: 3,
        title: ' Nike Blazer Mid Suede',
        price: 8499,
        imageUrl: '/sneakers/sneakers-3.jpg',
        isFavorite: true,
        favoriteId: 2,
        isAdded: false
      },
      3: {
        id: 4,
        title: ' Puma X Aka Boku Future Rider',
        price: 7800,
        imageUrl: '/sneakers/sneakers-4.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      4: {
        id: 5,
        title: ' Future Rider',
        price: 9550,
        imageUrl: '/sneakers/sneakers-5.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      5: {
        id: 6,
        title: ' Black Edition',
        price: 16999,
        imageUrl: '/sneakers/sneakers-6.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      6: {
        id: 7,
        title: ' Orange Boomb Edition',
        price: 7499,
        imageUrl: '/sneakers/sneakers-7.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      7: {
        id: 8,
        title: ' Nike Air Max 270',
        price: 15600,
        imageUrl: '/sneakers/sneakers-8.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      8: {
        id: 9,
        title: ' Nike Air Force 1',
        price: 5900,
        imageUrl: '/sneakers/sneakers-9.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      9: {
        id: 10,
        title: ' Adidas Ultraboost',
        price: 11500,
        imageUrl: '/sneakers/sneakers-10.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      10: {
        id: 11,
        title: ' Puma Clyde All-Pro',
        price: 7600,
        imageUrl: '/sneakers/sneakers-11.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      11: {
        id: 12,
        title: ' Converse Chuck Taylor All-Star',
        price: 13000,
        imageUrl: '/sneakers/sneakers-12.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      12: {
        name: 'Root',
        email: 'admin@email.com',
        id: 13,
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      13: { id: 14, isFavorite: false, favoriteId: null, isAdded: false },
      id: 15
    },
    {
      0: {
        id: 1,
        title: ' Nike Blazer Mid Suede',
        price: 12999,
        imageUrl: '/sneakers/sneakers-1.jpg',
        isFavorite: true,
        favoriteId: 3,
        isAdded: false
      },
      1: {
        id: 2,
        title: ' Nike Air Max 270',
        price: 15600,
        imageUrl: '/sneakers/sneakers-2.jpg',
        isFavorite: true,
        favoriteId: 1,
        isAdded: false
      },
      2: {
        id: 3,
        title: ' Nike Blazer Mid Suede',
        price: 8499,
        imageUrl: '/sneakers/sneakers-3.jpg',
        isFavorite: true,
        favoriteId: 2,
        isAdded: false
      },
      3: {
        id: 4,
        title: ' Puma X Aka Boku Future Rider',
        price: 7800,
        imageUrl: '/sneakers/sneakers-4.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      4: {
        id: 5,
        title: ' Future Rider',
        price: 9550,
        imageUrl: '/sneakers/sneakers-5.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      5: {
        id: 6,
        title: ' Black Edition',
        price: 16999,
        imageUrl: '/sneakers/sneakers-6.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      6: {
        id: 7,
        title: ' Orange Boomb Edition',
        price: 7499,
        imageUrl: '/sneakers/sneakers-7.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      7: {
        id: 8,
        title: ' Nike Air Max 270',
        price: 15600,
        imageUrl: '/sneakers/sneakers-8.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      8: {
        id: 9,
        title: ' Nike Air Force 1',
        price: 5900,
        imageUrl: '/sneakers/sneakers-9.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      9: {
        id: 10,
        title: ' Adidas Ultraboost',
        price: 11500,
        imageUrl: '/sneakers/sneakers-10.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      10: {
        id: 11,
        title: ' Puma Clyde All-Pro',
        price: 7600,
        imageUrl: '/sneakers/sneakers-11.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      11: {
        id: 12,
        title: ' Converse Chuck Taylor All-Star',
        price: 13000,
        imageUrl: '/sneakers/sneakers-12.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      id: 16
    },
    {
      0: {
        id: 1,
        title: ' Nike Blazer Mid Suede',
        price: 12999,
        imageUrl: '/sneakers/sneakers-1.jpg',
        isFavorite: true,
        favoriteId: 3,
        isAdded: false
      },
      1: {
        id: 2,
        title: ' Nike Air Max 270',
        price: 15600,
        imageUrl: '/sneakers/sneakers-2.jpg',
        isFavorite: true,
        favoriteId: 1,
        isAdded: false
      },
      2: {
        id: 3,
        title: ' Nike Blazer Mid Suede',
        price: 8499,
        imageUrl: '/sneakers/sneakers-3.jpg',
        isFavorite: true,
        favoriteId: 2,
        isAdded: false
      },
      3: {
        id: 4,
        title: ' Puma X Aka Boku Future Rider',
        price: 7800,
        imageUrl: '/sneakers/sneakers-4.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      4: {
        id: 5,
        title: ' Future Rider',
        price: 9550,
        imageUrl: '/sneakers/sneakers-5.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      5: {
        id: 6,
        title: ' Black Edition',
        price: 16999,
        imageUrl: '/sneakers/sneakers-6.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      6: {
        id: 7,
        title: ' Orange Boomb Edition',
        price: 7499,
        imageUrl: '/sneakers/sneakers-7.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      7: {
        id: 8,
        title: ' Nike Air Max 270',
        price: 15600,
        imageUrl: '/sneakers/sneakers-8.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      8: {
        id: 9,
        title: ' Nike Air Force 1',
        price: 5900,
        imageUrl: '/sneakers/sneakers-9.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      9: {
        id: 10,
        title: ' Adidas Ultraboost',
        price: 11500,
        imageUrl: '/sneakers/sneakers-10.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      10: {
        id: 11,
        title: ' Puma Clyde All-Pro',
        price: 7600,
        imageUrl: '/sneakers/sneakers-11.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      11: {
        id: 12,
        title: ' Converse Chuck Taylor All-Star',
        price: 13000,
        imageUrl: '/sneakers/sneakers-12.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      id: 17
    },
    {
      0: {
        id: 1,
        title: ' Nike Blazer Mid Suede',
        price: 12999,
        imageUrl: '/sneakers/sneakers-1.jpg',
        isFavorite: true,
        favoriteId: 3,
        isAdded: false
      },
      1: {
        id: 2,
        title: ' Nike Air Max 270',
        price: 15600,
        imageUrl: '/sneakers/sneakers-2.jpg',
        isFavorite: true,
        favoriteId: 1,
        isAdded: false
      },
      2: {
        id: 3,
        title: ' Nike Blazer Mid Suede',
        price: 8499,
        imageUrl: '/sneakers/sneakers-3.jpg',
        isFavorite: true,
        favoriteId: 2,
        isAdded: false
      },
      3: {
        id: 4,
        title: ' Puma X Aka Boku Future Rider',
        price: 7800,
        imageUrl: '/sneakers/sneakers-4.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      4: {
        id: 5,
        title: ' Future Rider',
        price: 9550,
        imageUrl: '/sneakers/sneakers-5.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      5: {
        id: 6,
        title: ' Black Edition',
        price: 16999,
        imageUrl: '/sneakers/sneakers-6.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      6: {
        id: 7,
        title: ' Orange Boomb Edition',
        price: 7499,
        imageUrl: '/sneakers/sneakers-7.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      7: {
        id: 8,
        title: ' Nike Air Max 270',
        price: 15600,
        imageUrl: '/sneakers/sneakers-8.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      8: {
        id: 9,
        title: ' Nike Air Force 1',
        price: 5900,
        imageUrl: '/sneakers/sneakers-9.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      9: {
        id: 10,
        title: ' Adidas Ultraboost',
        price: 11500,
        imageUrl: '/sneakers/sneakers-10.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      10: {
        id: 11,
        title: ' Puma Clyde All-Pro',
        price: 7600,
        imageUrl: '/sneakers/sneakers-11.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      11: {
        id: 12,
        title: ' Converse Chuck Taylor All-Star',
        price: 13000,
        imageUrl: '/sneakers/sneakers-12.jpg',
        isFavorite: false,
        favoriteId: null,
        isAdded: false
      },
      id: 18
    },
    { id: 19 }
  ]
]
</script>

<template>
  <!-- <Drawer /> -->
  <div class="bg-white w-4/5 m-auto rounded-xl shadow-xl mt-14">
    <Header />
    <div class="p-10">
      <div class="flex justify-between items-center">
        <h2 class="text-3xl font-bold mb-8">Всі Кросівки</h2>

        <div class="flex gap-4">
          <select class="py-2 px-3 border rounded-md outline-none">
            <option>За назвою</option>
            <option>За ціною (недорогі)</option>
            <option>За ціною (дорогі)</option>
          </select>
          <div class="relative">
            <img class="absolute left-4 top-3" src="/search.svg" />
            <input
              class="border rounded-md py-2 pl-11 pr-4 outline-none"
              type="text"
              placeholder="Пошук..."
            />
          </div>
        </div>
      </div>

      <CardList :items="items" />
    </div>
  </div>
</template>
