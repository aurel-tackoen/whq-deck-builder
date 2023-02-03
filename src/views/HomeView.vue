<script setup>
  const cardAmount = 15;
</script>
<template>
  <main>
    <h1 class="text-3xl font-bold underline">Hello world!</h1>
    <div class="cards">
      <div
        v-for="index in cardAmount"
        :key="index"
        class="card down"
        :style="`transform: rotateX(60deg) rotateY(0deg) rotateZ(5deg) translateZ(${
          index * 3
        }px)`"
      ></div>
    </div>
  </main>
</template>
