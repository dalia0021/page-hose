<script setup lang="ts">

</script>

<template>
  <section class="bg-amber-300 px-16 py-8 ">
    <div class="flex sm:max-w-[50%]">
      <img src="@/assets/specimen-vertical-B.svg" alt="">
      <img src="@/assets/specimen-vertical-A.svg" alt="">
    </div>
  </section>
</template>

<style scoped>
  @media (min-width: 64em) and (min-height: 36em) and (min-aspect-ratio: 6 / 5){
    img {
      height: calc(100vh - 4em);
      max-width: none;
    }
  }

</style>
