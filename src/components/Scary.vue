<template>
  <div class="grid grid-cols-1 xl:grid-cols-2 mt-16">
    <!-- Left -->
    <div class="xl:w-3/5 space-y-6 mt-32">
      <div class="text-white text-4xl font-semibold">
        NFTs Are not The Future Cannot Be Scary
      </div>
      <div class="text-gray-500 text-sm">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque
        euismod, nisi eu consectetur consectetur, nisl nisi consectetur nisi,
        euismod nisi nisi euismod nisi.
      </div>
      <div class="flex h-10">
        <input
          class="shadow bg-transparent appearance-none border rounded-lg w-64 py-2 px-3 text-gray-100 leading-tight focus:outline-none focus:shadow-outline mr-1"
          id="email"
          type="text"
          placeholder="Enter your email"
        />
        <Button :name="'Send'" :is_button_half_rounded="false" />
      </div>
    </div>

    <!-- Right -->
    <div class="block sm:flex mt-20 mx-auto">
      <Card
        v-for="item in items"
        :key="item.id"
        :price="item.price"
        :sub_price="item.sub_price"
        :status="item.status"
        :image="item.image"
        :style="`${
          getIndex(item.id) == 0
            ? '-ms-transfrom: skewX(170deg); transform: skewX(190deg);'
            : '-ms-transfrom: rotate(20deg); transform: rotate(20deg);'
        } background-color: black; width: 280px;`"
      />
    </div>
  </div>
</template>

<script setup>
import Button from '@/components/Button/Button.vue'
import Card from './card/Card.vue'
import { ref } from 'vue'

let items = ref([
  {
    id: 0,
    price: '1.26 ETH',
    sub_price: '$15253.13',
    status: 'Current Price',
    image: 'one',
  },
  {
    id: 1,
    price: '1.27 ETH',
    sub_price: '$15253.13',
    status: 'Current Price',
    image: 'two',
  },
])

// get array index of item with id of 0
const getIndex = (id) => items.value.findIndex((item) => item.id === id)
</script>
