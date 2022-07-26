<script setup lang="ts">
import Inicio from "@/components/Inicio.vue"
import SeccionDos from "@/components/SeccionDos.vue"
import SeccionTres from "@/components/SeccionTres.vue"
import SeccionCuatro from "@/components/SeccionCuatro.vue"
import SeccionSinco from "@/components/SeccionSinco.vue"
import SeccionSeis from "@/components/SeccionSeis.vue"
import SeccionSiete from "@/components/SeccionSiete.vue"
import SeccionOcho from "@/components/SeccionOcho.vue"
import SeccionNueve from "@/components/SeccionNueve.vue"
import SeccionDiez from "@/components/SeccionDiez.vue"
import SeccionOnce from "@/components/SeccionOnce.vue"
import SeccionDoce from "@/components/SeccionDoce.vue"
import SeccionTrece from "@/components/SeccionTrece.vue"
import Fin from "@/components/Fin.vue"


import { ref } from 'vue'

 const scrollContainer = ref<null | { scrollLeft: () => null }>(null)

const scrollH = (evt: any) => {
  if(scrollContainer.value){
    scrollContainer.value.scrollLeft += evt.deltaY;
  }
} 

</script>

<template>
<article @wheel.prevent="scrollH" ref="scrollContainer" class="lg:h-screen lg:overflow-x-scroll lg:overflow-y-hidden lg:whitespace-nowrap">
  <Inicio class="lg:overflow-y-auto lg:inline-block lg:max-w-[115vh] h-screen"/>  
  <SeccionDos class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionTres class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionCuatro class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionSinco class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionSeis class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionSiete class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionOcho class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionNueve class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionDiez class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionOnce class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionDoce class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <SeccionTrece class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
  <Fin class="lg:overflow-y-auto lg:inline-block lg:h-screen"/>
</article>
</template>

<style>




</style>
