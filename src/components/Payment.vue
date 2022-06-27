<script setup>
import Card from './card/Card.vue'
import { ref } from 'vue'

let items = ref([
  {
    id: 0,
    name: 'BINANCE',
    image: 'binance.png',
  },
  {
    id: 1,
    name: 'PayPal',
    image: 'paypal.jfif',
  },
  {
    id: 2,
    name: 'METAMASK',
    image: 'metamask.png',
  },
  {
    id: 3,
    name: 'VINTAGE',
    image: 'V.jpg',
  },
  {
    id: 4,
    name: 'StoneTech',
    image: 'stonetech.jfif',
  },
  {
    id: 5,
    name: 'CAMPFIRE',
    image: 'campfire.jfif',
  },
])
</script>
<template>
  <div class="flex justify-center mt-14">
    <div class="grid grid-cols-2 md:grid-cols-5 lg:grid-cols-6 gap-20">
      <div
        v-for="item in items"
        :key="item.id"
        class="flex grayscale opacity-60"
      >
        <img
          class="w-5 h-5 mr-2"
          :src="`/src/assets/images/${item.image}`"
          alt=""
        />
        <span class="text-white text-sm font-bold">{{ item.name }}</span>
      </div>
    </div>
  </div>
</template>
