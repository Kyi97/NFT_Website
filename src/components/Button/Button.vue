<template>
  <button
    :class="`px-4 py-2 flex bg-gradient-to-r from-red-500 to-pink-600 text-white text-sm font-medium
    hover:from-red-600 hover:to-pink-700 hover:scale-105 ease-in duration-100 transition cursor-pointer
    active:from-red-500 active:to-pink-600
     ${is_button_half_rounded ? 'rounded-tl-xl rounded-br-xl' : 'rounded-md'}`"
  >
    {{ name }}
  </button>
</template>

<script setup>
defineProps({
  name: {
    type: String,
    required: true,
  },
  is_button_half_rounded: {
    type: Boolean,
    required: true,
  },
})
</script>
