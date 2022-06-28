<template>
  <div class="relative border-2 border-[#494948] rounded-2xl mx-4 my-3">
    <div
      class="bg-[#585857] opacity-50 w-full h-full absolute blur-md bg-transparent"
    ></div>
    <div
      class="relative p-4 w-full bg-transparent rounded-lg overflow-hidden shadow"
      style="min-height: 160px"
    >
      <div>
        <div class="relative h-full flex justify-center">
          <img
            class="rounded-xl w-full aspect-[4/2] object-cover object-top"
            :src="image"
          />
          <div class="absolute w-[88%]">
            <div
              class="relative w-full h-[1.8rem] flex justify-center items-center"
            >
              <div
                class="bg-black w-full h-[1.9rem] absolute rounded-t-[0.4rem]"
                style="-webkit-transform: perspective(100px) rotateX(162deg)"
              ></div>
              <p
                class="absolute text-zinc-300 text-sm font-bold text-center top-[.2rem]"
              >
                {{ header }}
              </p>
            </div>
          </div>
          <div class="h-8 absolute bottom-0 p-1">
            <img
              class="rounded-full w-14 border-[3px] border-black"
              :src="creator_image"
            />
          </div>
        </div>
      </div>
      <div class="flex flex-col items-center mt-9">
        <div class="text-white font-semibold">Created By {{ created_by }}</div>
        <div class="flex items-center pb-3">
          <div class="text-pink-600 text-base">{{ price }} &nbsp;</div>
          <div class="text-gray-300 text-sm">Artwork</div>
        </div>
        <Button
          :name="'+Following'"
          :is_button_half_rounded="false"
          :padding_y="'4.5px'"
          :padding_x="'55px'"
        />
        <!-- <h2
          class="mt-2 text-transparent bg-clip-text bg-gradient-to-r from-red-500 to-pink-600 text-base font-bold"
        >
          xaxax
          <span class="text-xs mt-2 text-zinc-300 line-clamp-1">xaxax</span>
        </h2>

        <Button :name="'Bid Now'" :is_button_half_rounded="true" /> -->
      </div>
    </div>
  </div>
</template>

<script setup>
import Button from '../Button/Button.vue'
defineProps({
  header: {
    type: String,
    required: true,
  },
  created_by: {
    type: String,
    required: true,
  },
  price: {
    type: String,
    required: true,
  },
  image: {
    type: String,
    required: true,
  },
  creator_image: {
    type: String,
    required: true,
  },
})
</script>
