<script setup>
defineProps({
  price: {
    type: String,
    required: true,
  },
  status: {
    type: String,
  },
  image: {
    type: Image,
    required: true,
  },
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
    <p class="mt-2 text-gray-800 text-sm">{{ status }}</p>
    <h2 class="mt-2 text-gray-800 text-sm font-semibold line-clamp-1">
      {{ price }}
    </h2>

    <button
      class="
        mt-4
        px-4
        py-2
        bg-indigo-500
        hover:bg-indigo-600
        text-white text-sm
        font-medium
        rounded-md
        w-full
      "
    >
      Bid Now
    </button>
  </div>
</template>