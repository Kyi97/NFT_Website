<script setup>
// function getImageUrl(image) {
//   return new URL(`../../assets/images/${image}.jpg`, import.meta.url).href
// }
defineProps({
  price: {
    type: String,
    required: true,
  },
  sub_price: {
    type: String,
    required: true,
  },
  status: {
    type: String,
  },
  image: {
    type: String,
  },
});
</script>

<template>
  <div class="relative border-2 border-[#494948] rounded-xl ">
    <div
      class="bg-[#585857] opacity-50 w-full h-full absolute blur-md bg-transparent"
    ></div>
    <div
      class="
        relative
        p-4
        w-full
        bg-transparent
        rounded-lg
        overflow-hidden
        shadow
      "
      style="min-height: 160px"
    >
      <div>
        <div class="relative h-full flex justify-center">
          <img
            class="rounded-lg h-[30vh] w-full object-cover"
            :src="`src/assets/images/${image}.jpg`"
          />
          <div class="bg-black w-[90%] h-8 absolute top-0 p-1 rounded-b-full">
            <p class="text-zinc-300 text-sm font-bold text-center">
              Designpgh Club
            </p>
          </div>
          <div
            class="bg-black w-[65%] h-8 absolute bottom-0 p-1 rounded-t-full"
          >
            <p
              class="
                text-transparent
                bg-clip-text bg-gradient-to-r
                from-red-500
                to-pink-600
                text-sm
                font-bold
                text-center
              "
            >
              01h : 03m : 35s
            </p>
          </div>
        </div>
      </div>
      <p class="mt-2 text-zinc-300 text-sm">{{ status }}</p>
      <div class="flex justify-between">
        <h2
          class="
            mt-2
            text-transparent
            bg-clip-text bg-gradient-to-r
            from-red-500
            to-pink-600
            text-base
            font-bold
          "
        >
          {{ price }}
          <span class="text-xs mt-2 text-zinc-300 line-clamp-1">{{
            sub_price
          }}</span>
        </h2>

        <button
          class="
            px-4
            py-2
            bg-gradient-to-r
            from-red-500
            to-pink-600
            text-white text-sm
            font-medium
            rounded-tl-xl rounded-br-xl
          "
        >
          Bid Now
        </button>
      </div>
    </div>
  </div>
</template>
