<script setup>
defineProps({
  price: {
    type: String,
    required: true,
  },
  image:{
      type: Image,
      required: true
  }
});
</script>

<template>
  <div
    class="relative p-4 w-full bg-white rounded-lg overflow-hidden shadow"
    style="min-height: 160px"
  >
    <div>
      <div class="relative block h-full">
        <div class="h-32 bg-gray-100 rounded-lg"></div>
      </div>
    </div>

    <h2 class="mt-4 text-gray-800 text-sm font-semibold line-clamp-1">
      {{ price }}
    </h2>
  </div>
</template>