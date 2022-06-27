<script setup></script>
<template>
  <nav class="bg-black shadow-lg">
    <div class="max-w-6xl mx-auto px-4">
      <div class="flex justify-between">
        <!-- Website Logo -->
        <div>
          <a href="#" class="flex items-center py-4 px-2">
            <img
              src="/src/assets/images/wk.jpg"
              alt="Logo"
              class="h-8 w-8 mr-2 rounded-full"
            />
          </a>
        </div>
        <!-- Primary Navbar items -->
        <div class="hidden md:flex items-center space-x-5">
          <a
            href=""
            class="py-4 px-2 text-white border-b border-red-500 font-semibold"
            >Explore</a
          >
          <a
            href=""
            class="py-4 px-2 text-zinc-300 font-semibold hover:text-red-500 transition duration-300"
            >Collections</a
          >
          <a
            href=""
            class="py-4 px-2 text-zinc-300 font-semibold hover:text-red-500 transition duration-300"
            >Community</a
          >
          <a
            href=""
            class="py-4 px-2 text-zinc-300 font-semibold hover:text-red-500 transition duration-300"
            >Contact Us</a
          >
        </div>

        <div class="mt-5">
          <a href="#">
            <svg
              class="w-6 h-6 fill-white"
              stroke="white"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h8m-8 6h16"
              ></path>
            </svg>
          </a>
        </div>
      </div>
    </div>
  </nav>
</template>
