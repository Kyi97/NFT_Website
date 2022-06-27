<script setup>
import FilterButton from "@/components/FilterButton/FilterButton.vue";
import { ref } from "vue";
let items = ref([
  {
    id: 0,
    name: "Virtual World",
  },
  { id: 1, name: "Music" },
  { id: 2, name: "Building" },
  { id: 3, name: "Art" },
  { id: 4, name: "Trading Card" },
  { id: 5, name: "Hot" },
  { id: 6, name: "More >>" },
]);
</script>
<template>
  <div class="mt-20">
    <!-- Header -->
    <div class="flex flex-col items-center space-y-4">
      <div class="text-zinc-400 text-xs">NFT MARKETPLACE</div>
      <div class="text-white text-3xl font-bold">Explore Nft Marketplace</div>
      <div class="text-zinc-400 text-xs max-w-sm text-center">
        In Short Nfts Are Non-Fungible Tokens, Where Fungible Means Replaceable
        And Tokens Are Generally Assets
      </div>
    </div>

    <!-- Filter Buttons -->
    <div class="flex justify-center mt-14">
      <div class="grid grid-cols-4 md:grid-cols-6 lg:grid-cols-7 gap-3">
        <FilterButton
          v-for="item in items"
          :key="item.id"
          :name="item.name"
        ></FilterButton>
      </div>
    </div>
  </div>
</template>