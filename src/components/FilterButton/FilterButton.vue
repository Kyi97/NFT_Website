<template>
  <button
    :class="` bg-[#2c2c2b] font-sm rounded-full text-sm py-2.5 px-3
     ${
       name == 'Art'
         ? 'bg-gradient-to-r from-red-500 to-pink-600 text-white'
         : 'text-zinc-400 bg-[#2c2c2b]'
     }`"
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
});
</script>
