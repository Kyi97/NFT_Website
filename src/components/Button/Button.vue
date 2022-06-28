<template>
  <button
    :class="`flex bg-gradient-to-r from-red-500 to-pink-600 text-white text-sm font-medium
      hover:from-red-600 hover:to-pink-700 hover:scale-105 ease-in duration-100 transition cursor-pointer
      active:from-red-500 active:to-pink-600 py-2 px-4
       ${is_button_half_rounded ? 'rounded-tl-xl rounded-br-xl' : 'rounded-md'}
       `"
  >
    {{ name }}
  </button>
</template>
<!-- ${width ? get_width(width) : ''}
       ${padding_y ? get_padding_y(padding_y) : 'py-2'}
       ${padding_x ? get_padding_x(padding_x) : 'px-4'} -->

<script setup>
// function get_width(v) {
//   return `w-[${v}]`
// }
// function get_padding_x(v) {
//   if (v) {
//     return `px-[${v}]`
//   } else {
//     return ''
//   }
// }
// function get_padding_y(v) {
//   if (v) {
//     return `py-[${v}]`
//   } else {
//     return ''
//   }
// }
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
