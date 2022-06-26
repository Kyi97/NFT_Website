<template>
  <div class="mt-20">
    <!-- Header -->
    <div class="flex flex-col items-center space-y-4">
      <div class="text-gray-400 text-xs">NFT MARKETPLACE</div>
      <div class="text-white text-3xl font-bold">Top Vendor In A Week</div>
      <div class="text-gray-400 text-xs max-w-sm text-center">
        lorem ipsum dolor sit amet consectetur adipisicing elit sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua
      </div>
    </div>

    <!-- VendorCard -->
    <div
      class="grid sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-2 xl:grid-cols-3 2xl:grid-cols-4 text-white mt-9"
    >
      <VendorCard
        v-for="vendor in vendors"
        :key="vendor.id"
        :name="vendor.name"
        :type="vendor.type"
        :image="vendor.image"
        :income="vendor.income"
        :outcome="vendor.outcome"
      />
    </div>
  </div>
</template>

<script setup>
import VendorCard from '@/components/VendorCard/VendorCard.vue'
import { ref } from 'vue'

let vendors = ref([
  {
    id: 0,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 1,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/mandalorian-fan-art-5k-fq-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 2,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/katee-sackhoff-as-bo-katan-kryze-the-mandalorian-sr-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 3,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/arcane-jinx-fanart-4k-bp-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 4,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/the-batman-2022-10k-hq-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 5,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/moon-knight-tv-series-5k-2t-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 6,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/the-moon-knight-w5-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 7,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/the-dark-knight-superhero-9u-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 8,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/vision-from-wandavision-qh-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 9,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/what-if-vision-4k-j3-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 10,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/anya-taylor-joy-the-northman-event-4k-o2-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 11,
    name: 'Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/samurai-assassins-creed-4-black-flag-ry-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
])
</script>
