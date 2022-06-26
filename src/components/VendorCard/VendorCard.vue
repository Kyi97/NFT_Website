<template>
  <div
    class="flex justify-between border-2 border-gray-700 rounded-lg px-4 py-2 bg-black mx-4 mt-6"
  >
    <div>
      <img :src="image" class="rounded-full w-10 h-10 object-cover" />
    </div>
    <div class="w-[50%] space-y-1">
      <div class="text-sm">{{ name }}</div>
      <div class="text-gray-400 text-xs">{{ type }}</div>
    </div>
    <div class="space-y-2 text-xs">
      <div class="text-green-600">{{ income }}</div>
      <div class="text-red-600">{{ outcome }}</div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  name: {
    type: String,
    required: true,
  },
  type: {
    type: String,
    required: true,
  },
  image: {
    type: String,
    required: true,
  },
  income: {
    type: String,
    required: true,
  },
  outcome: {
    type: String,
    required: true,
  },
})
</script>
