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
      <ArtistCard />
      <ArtistCard />
      <ArtistCard />
      <ArtistCard />
    </div>
  </div>
</template>

<script setup>
import ArtistCard from './ArtistCard/ArtistCard.vue'
</script>
