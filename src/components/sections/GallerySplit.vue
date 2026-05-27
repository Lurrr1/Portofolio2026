<template>
  <section
    class="relative w-full h-screen bg-[#ebebeb] overflow-hidden select-none flex items-center justify-center"
  >
    <BlueprintRuler position="top" :marker-index="20" class="z-50" />
    <BlueprintRuler position="bottom" :marker-index="140" class="z-50" />

    <div class="absolute inset-0 z-40 flex flex-col md:flex-row pointer-events-none">
      <div class="w-full md:w-1/2 h-full flex items-center justify-center relative p-8 lg:p-12">
        <div
          class="absolute top-12 left-12 text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 z-50"
        >
          UI/UX Design
        </div>

        <div
          class="relative w-[55%] max-w-[320px] aspect-square rounded-sm overflow-hidden shadow-2xl hover:scale-105 transition-transform duration-700 cursor-pointer pointer-events-auto z-40 ring-1 ring-neutral-400/50"
        >
          <img
            src="https://images.unsplash.com/photo-1618761714954-0b8cd0026356?q=80&w=2070&auto=format&fit=crop"
            alt="AgroSmart UI Interface"
            class="w-full h-full object-cover grayscale hover:grayscale-0 transition-all duration-500"
          />
        </div>
      </div>

      <div class="relative w-full md:w-1/2 h-full overflow-hidden pointer-events-auto z-40">
        <div
          class="absolute top-12 right-12 text-[11px] font-bold tracking-widest text-white z-50 mix-blend-difference"
        >
          05
        </div>

        <img
          src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?q=80&w=2070&auto=format&fit=crop"
          alt="IoT Spatial Analysis Dashboard"
          class="w-full h-full object-cover grayscale hover:grayscale-0 transition-all duration-700"
        />
      </div>

      <div
        class="absolute top-0 bottom-0 left-1/2 w-px bg-neutral-300/50 z-50 hidden md:block"
      ></div>
    </div>

    <div class="absolute inset-0 m-8 pointer-events-none z-50">
      <BlueprintGrid
        :rows="3"
        :cols="5"
        :white-markers="[6, 2, 3, 4, 7, 8, 9, 12, 13, 14]"
        :black-markers="[0, 1, 5, 10, 11]"
      />
    </div>
  </section>
</template>

<script setup>
import BlueprintGrid from '../ui/BlueprintGrid.vue'
import BlueprintRuler from '../ui/BlueprintRuler.vue'
</script>
