<script setup>
import Card from "./card/Card.vue";
import { ref } from "vue";

let items = ref([
  {
    id: 0,
    price: "1.26 ETH",
    sub_price: "$15253.13",
    status: "Current Price",
    image: "./src/assets/images/one.jpg",
  },
  {
    id: 1,
    price: "1.27 ETH",
    sub_price: "$15253.13",
    status: "Current Price",
    image: "./src/assets/images/two.jpg",
  },
  {
    id: 2,
    price: "1.28 ETH",
    sub_price: "$15253.13",
    status: "Current Price",
    image: "./src/assets/images/three.jpg",
  },
  {
    id: 3,
    price: "1.29 ETH",
    sub_price: "$15253.13",
    status: "Current Price",
    image: "./src/assets/images/four.jpg",
  },
  {
    id: 4,
    price: "1.26 ETH",
    sub_price: "$15253.13",
    status: "Current Price",
    image: "./src/assets/images/five.jpg",
  },
  {
    id: 5,
    price: "1.27 ETH",
    sub_price: "$15253.13",
    status: "Current Price",
    image: "./src/assets/images/six.jpg",
  },
  {
    id: 6,
    price: "1.28 ETH",
    sub_price: "$15253.13",
    status: "Current Price",
    image: "./src/assets/images/seven.jpg",
  },
  {
    id: 7,
    price: "1.29 ETH",
    sub_price: "$15253.13",
    status: "Current Price",
    image: "./src/assets/images/eight.jpg",
  },
]);
</script>
<template>
  <div
    class="
      grid grid-cols-1
      md:grid-cols-2
      lg:grid-cols-3
      xl:grid-cols-3
      2xl:grid-cols-4
      gap-4
      w-full
      mt-10
    "
  >
    <Card
      v-for="item in items"
      :key="item.id"
      :price="item.price"
      :sub_price="item.sub_price"
      :status="item.status"
      :image="item.image"
    />
  </div>
</template>