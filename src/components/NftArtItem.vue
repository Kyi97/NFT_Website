<script setup>
import Card from "./card/Card.vue";
</script>
<template>
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4 w-full">
    <Card price="0.25 ETH " status="Current Price"/>
    <Card price="0.25 ETH " status="Current Price"/>
    <Card price="0.25 ETH " status="Current Price"/>
    <Card price="0.25 ETH " status="Current Price"/>
  </div>
</template>