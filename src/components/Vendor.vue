<template>
  <div class="mt-20">
    <div class="grid grid-cols-4 text-white">
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
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 1,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 2,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 3,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 4,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 5,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 6,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 7,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 8,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 9,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 10,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
  {
    id: 11,
    name: '>Marvin McKimmich',
    type: 'MOD Cretete',
    image:
      'https://images.hdqwalls.com/download/scarletwitch-doctor-strange-in-the-multiverse-of-madness-jd-240x240.jpg',
    income: '+399.4%',
    outcome: '-0.334%',
  },
])
</script>
