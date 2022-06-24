<script setup>
// function getImageUrl(image) {
//   return new URL(`../../assets/images/${image}.jpg`, import.meta.url).href
// }
defineProps({
  price: {
    type: String,
    required: true,
  },
  status: {
    type: String,
  },
  image: {
    type: String,
  },
})
</script>

<template>
  <div
    class="relative p-4 w-full bg-white rounded-lg overflow-hidden shadow"
    style="min-height: 160px"
  >
    <div>
      <div class="relative block h-full">
        <img
          class="rounded-lg h-32 w-full object-cover"
          :src="`src/assets/images/${image}.jpg`"
        />
      </div>
    </div>
    <p class="mt-2 text-gray-800 text-sm">{{ status }}</p>
    <div class="flex justify-between">
      <h2 class="mt-2 text-gray-800 text-sm font-semibold line-clamp-1">
        {{ price }}
      </h2>

      <button
        class="px-4 py-2 bg-gradient-to-r from-red-500 to-pink-600 text-white text-sm font-medium rounded-md"
      >
        Bid Now
      </button>
    </div>
  </div>
</template>
