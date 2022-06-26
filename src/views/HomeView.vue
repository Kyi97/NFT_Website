<script setup>
// import Test from "@/components/Test.vue";
import Payment from '@/components/Payment.vue'
import Filter from '@/components/Filter.vue'
import NftArtItem from '@/components/NftArtItem.vue'
import Scary from '@/components/Scary.vue'
import Footer from '@/components/Footer.vue'
import Vendor from '../components/Vendor.vue'
import Artist from '../components/Artist.vue'
</script>

<template>
  <main>
    <Payment class="px-7" />
    <Filter class="px-7" />
    <NftArtItem class="px-7 md:px-10 lg:px-24" />
    <Artist class="px-7 md:px-10 lg:px-24" />
    <Vendor class="px-7 md:px-10 lg:px-24" />
    <Scary class="px-7 md:px-10 lg:px-24" />
    <Footer />
  </main>
</template>

<style></style>
