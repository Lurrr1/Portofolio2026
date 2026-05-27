<template>
  <section class="relative w-full h-screen overflow-hidden select-none">
    <div class="absolute inset-0 z-0 group cursor-pointer pointer-events-auto overflow-hidden">
      <img
        src="https://images.unsplash.com/photo-1518770660439-4636190af475?q=80&w=2070&auto=format&fit=crop"
        alt="Featured Full-Bleed Visual"
        class="w-full h-full object-cover grayscale group-hover:grayscale-0 group-hover:scale-105 transition-all duration-1000"
      />
    </div>

    <BlueprintRuler position="top" :marker-index="70" class="z-20" />
    <BlueprintRuler position="bottom" :marker-index="110" class="z-20" />

    <div
      class="absolute top-12 left-12 text-[10px] font-bold uppercase tracking-[0.2em] z-40 pointer-events-none mix-blend-difference text-white"
    >
      Featured Visual
    </div>
    <div
      class="absolute top-12 right-12 text-[11px] font-bold tracking-widest z-40 pointer-events-none mix-blend-difference text-white"
    >
      06
    </div>

    <div class="absolute inset-0 pointer-events-none z-10">
      <BlueprintGrid :rows="3" :cols="5" :show-markers="false" />
    </div>

    <div class="absolute inset-0 pointer-events-none z-30">
      <BlueprintGrid
        :rows="3"
        :cols="5"
        :show-lines="false"
        :white-markers="[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14]"
      />
    </div>
  </section>
</template>

<script setup>
import BlueprintGrid from '../ui/BlueprintGrid.vue'
import BlueprintRuler from '../ui/BlueprintRuler.vue'
</script>
