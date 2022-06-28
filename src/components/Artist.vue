<template>
  <div class="mt-20">
    <!-- Header -->
    <div class="flex flex-col items-center space-y-4">
      <div class="text-gray-400 text-xs">CREATORS NFTS</div>
      <div class="text-white text-3xl font-bold">Top List Artist</div>
      <div class="text-gray-400 text-xs max-w-sm text-center">
        lorem ipsum dolor sit amet consectetur adipisicing elit sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua
      </div>
    </div>

    <!-- Card -->
    <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-4 mt-14">
      <ArtistCard
        v-for="item in items"
        :key="item.id"
        :header="item.header"
        :created_by="item.created_by"
        :price="item.price"
        :image="item.image"
        :creator_image="item.creator_image"
      />
    </div>
  </div>
</template>

<script setup>
import ArtistCard from './ArtistCard/ArtistCard.vue'
import { ref } from 'vue'
let items = ref([
  {
    id: 0,
    header: 'Designpgh Club',
    created_by: 'Kyi',
    price: '12.3K',
    image:
      'https://images.hdqwalls.com/download/spongebob-squarepants-4k-2020-4s-240x240.jpg',
    creator_image:
      'https://images.hdqwalls.com/download/motogp-2022-0g-240x240.jpg',
  },
  {
    id: 2,
    header: 'Designpgh Club',
    created_by: 'Sin',
    price: '12.3K',
    image:
      'https://images.hdqwalls.com/download/2022-the-wolf-among-us-2-5k-qu-240x240.jpg',
    creator_image:
      'https://images.hdqwalls.com/download/fallout-game-concept-art-5k-u2-240x240.jpg',
  },
  {
    id: 3,
    header: 'Designpgh Club',
    created_by: 'Thant',
    price: '12.3K',
    image:
      'https://images.hdqwalls.com/download/elder-scrolls-online-5k-bn-240x240.jpg',
    creator_image:
      'https://images.hdqwalls.com/download/spiderman-miles-morales-kick-5k-jc-240x240.jpg',
  },
  {
    id: 4,
    header: 'Designpgh Club',
    created_by: 'NFT',
    price: '12.3K',
    image:
      'https://images.hdqwalls.com/download/runied-king-a-league-of-legends-ml-240x240.jpg',
    creator_image:
      'https://images.hdqwalls.com/download/what-if-vision-4k-j3-240x240.jpg',
  },
])
</script>
