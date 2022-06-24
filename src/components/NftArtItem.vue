<script setup>
import Card from "./card/Card.vue";
import { ref } from "vue";

let items = ref([
  {
    id: 0,
    price: "1.26 ETH",
    sub_price:"$15253.13",
    status: "Current Price",
    image: "one",
  },
  {
    id: 1,
    price: "1.27 ETH",
    sub_price:"$15253.13",
    status: "Current Price",
    image: "two",
  },
  {
    id: 2,
    price: "1.28 ETH",
    sub_price:"$15253.13",
    status: "Current Price",
    image: "three",
  },
  {
    id: 3,
    price: "1.29 ETH",
    sub_price:"$15253.13",
    status: "Current Price",
    image: "four",
  },
  {
    id: 4,
    price: "1.26 ETH",
    sub_price:"$15253.13",
    status: "Current Price",
    image: "five",
  },
  {
    id: 5,
    price: "1.27 ETH",
    sub_price:"$15253.13",
    status: "Current Price",
    image: "six",
  },
  {
    id: 6,
    price: "1.28 ETH",
    sub_price:"$15253.13",
    status: "Current Price",
    image: "seven",
  },
  {
    id: 7,
    price: "1.29 ETH",
    sub_price:"$15253.13",
    status: "Current Price",
    image: "eight",
  },
]);
</script>
<template>
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4 w-full">
    <Card
      v-for="item in items"
      :key="item.id"
      :price="item.price"
      :status="item.status"
      :image="item.image"
    />
  </div>
</template>