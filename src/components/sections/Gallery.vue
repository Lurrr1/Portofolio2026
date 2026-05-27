<template>
  <section class="relative w-full h-screen bg-[#1a1a1a] overflow-hidden select-none">
    <BlueprintRuler position="top" :marker-index="90" class="z-40" />
    <BlueprintRuler position="bottom" :marker-index="120" class="z-40" />

    <div
      class="absolute top-12 left-12 text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 z-40 mix-blend-difference text-white pointer-events-none"
    >
      Visual Documentation
    </div>

    <div
      class="absolute top-12 right-12 text-[11px] font-bold tracking-widest text-neutral-900 z-40 mix-blend-difference text-white pointer-events-none"
    >
      04
    </div>

    <div
      class="absolute inset-0 z-0 grid gap-0"
      style="
        grid-template-columns: calc(25% + 1rem) calc(25% - 1rem) calc(25% - 1rem) calc(25% + 1rem);
        grid-template-rows: 50% 50%;
      "
    >
      <router-link
        to="/project/empathetic-ai"
        class="relative overflow-hidden grayscale hover:grayscale-0 transition-all duration-700 cursor-pointer group block"
      >
        <img
          src="D:\Vue\Porto\public\images\Sempro.webp"
          alt="Empathetic AI Assistant"
          class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
        />
      </router-link>

      <router-link
        to="/project/carbon-detection"
        class="relative overflow-hidden grayscale hover:grayscale-0 transition-all duration-700 cursor-pointer group block"
      >
        <img
          src="D:\Vue\Porto\public\images\Sensing.webp"
          alt="PM 2.5 Carbon Detection"
          class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
        />
      </router-link>

      <router-link
        to="/project/groot-chairman"
        class="col-span-2 relative overflow-hidden grayscale hover:grayscale-0 transition-all duration-700 cursor-pointer group block"
      >
        <img
          src="D:\Vue\Porto\public\images\Groot.webp"
          alt="Groot UIR Chairman"
          class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
        />
      </router-link>

      <router-link
        to="/project/bangkit-academy"
        class="relative overflow-hidden grayscale hover:grayscale-0 transition-all duration-700 cursor-pointer group block"
      >
        <img
          src="D:\Vue\Porto\public\images\Team1.webp"
          alt="Bangkit Academy"
          class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
        />
      </router-link>

      <router-link
        to="/project/water-turbidity-iot"
        class="relative overflow-hidden grayscale hover:grayscale-0 transition-all duration-700 cursor-pointer group block"
      >
        <img
          src="https://images.unsplash.com/photo-1581091226825-a6a2a5aee158?q=80&w=2070&auto=format&fit=crop"
          alt="Water Turbidity IoT System"
          class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
        />
      </router-link>

      <router-link
        to="/project/earthquake-analysis"
        class="relative overflow-hidden grayscale hover:grayscale-0 transition-all duration-700 cursor-pointer group block"
      >
        <img
          src="https://images.unsplash.com/photo-1527443224154-c4a3942d3acf?q=80&w=2070&auto=format&fit=crop"
          alt="Spatial Earthquake Analysis"
          class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
        />
      </router-link>

      <router-link
        to="/project/forest-fire-forecasting"
        class="relative overflow-hidden grayscale hover:grayscale-0 transition-all duration-700 cursor-pointer group block"
      >
        <img
          src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?q=80&w=2070&auto=format&fit=crop"
          alt="Forest Fire Hotspot Forecasting"
          class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
        />
      </router-link>
    </div>

    <div class="absolute inset-0 m-8 pointer-events-none z-30">
      <BlueprintGrid
        :rows="3"
        :cols="5"
        :white-markers="[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14]"
      />
    </div>
  </section>
</template>

<script setup>
import BlueprintGrid from '../ui/BlueprintGrid.vue'
import BlueprintRuler from '../ui/BlueprintRuler.vue'
</script>
