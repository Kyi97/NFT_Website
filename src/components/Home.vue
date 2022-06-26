<script setup>
import Button from "@/components/Button/Button.vue";
</script>
<template>
  <div class="grid grid-cols-1 xl:grid-cols-2 space-x-14">
    <div class="space-y-6 mt-20">
      <div class="text-zinc-400 text-sm font-semibold">NFT MARKET PLACE!</div>
      <div class="text-white text-5xl leading-snug">
        The <span class="underline font-bold">Most</span> <br />
        Interesting Digital<br />
        In The
        <span
          class="
            text-transparent
            bg-clip-text bg-gradient-to-r
            from-red-500
            to-pink-600
            font-bold
          "
          >World</span
        >
      </div>
      <div class="text-zinc-400 text-sm font-semibold">
        In short NFTs are
        <span
          class="
            text-transparent
            bg-clip-text bg-gradient-to-r
            from-red-500
            to-pink-600
            font-bold
          "
          >Non-fungible tokens</span
        >, where fungible means replaceable are generally assets soon you will
        be able to enjoy the best way to monetize your Christmas NFTs are coming
      </div>
      <div class="flex h-10">
        <Button :name="'Explore Now'" :is_button_half_rounded="true" />
        <div class="flex ml-5 mt-2">
          <svg
            class="w-6 h-6 text-red-500"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              class="text-white"
              fill="none"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"
            ></path>
            <path
              class="bg-red"
              fill="none"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
            ></path>
          </svg>
          <span class="text-zinc-400 text-sm font-bold ml-3"
            >Demo Explore Now</span
          >
        </div>
      </div>
    </div>

    <div class="flex mx-auto mt-16">
      <img
        class="rounded-lg h-96 w-full object-cover"
        src="src/assets/images/four.jpg"
      />
    </div>
  </div>
</template>

