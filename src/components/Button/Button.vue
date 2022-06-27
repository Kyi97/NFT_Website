<template>
  <button
    :class="`flex bg-gradient-to-r from-red-500 to-pink-600 text-white text-sm font-medium
      hover:from-red-600 hover:to-pink-700 hover:scale-105 ease-in duration-100 transition cursor-pointer
      active:from-red-500 active:to-pink-600
       ${is_button_half_rounded ? 'rounded-tl-xl rounded-br-xl' : 'rounded-md'}
       ${width ? `w-[${width}]` : ''}
       ${padding_y ? `py-[${padding_y}]` : 'py-2'}
       ${padding_x ? `px-[${padding_x}]` : 'px-4'}
       `"
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
  width: {
    type: String,
    required: false,
  },
  padding_y: {
    type: String,
    required: false,
  },
  padding_x: {
    type: String,
    required: false,
  },
})
</script>
