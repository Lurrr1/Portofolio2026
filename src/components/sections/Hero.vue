<template>
  <section
    class="relative w-full h-screen bg-[#ebebeb] text-[#1a1a1a] font-sans overflow-hidden select-none flex items-center justify-center"
  >
    <BlueprintRuler position="bottom" :marker-index="10" />

    <div
      class="absolute inset-0 flex flex-col justify-between pointer-events-none select-none py-16 md:py-16 opacity-[0.03]"
    >
      <h2 class="text-[18vw] font-serif tracking-tight text-center leading-none">Portfolio</h2>
      <h2 class="text-[18vw] font-serif tracking-tight text-center leading-none">Portfolio</h2>
    </div>

    <div class="relative z-10 text-center px-4 mix-blend-multiply pointer-events-none">
      <h1
        class="text-[13vw] sm:text-[11vw] font-serif tracking-tight text-neutral-900 leading-none drop-shadow-sm filter contrast-125"
      >
        Portfolio
      </h1>
    </div>

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none">
      <BlueprintGrid :rows="3" :cols="5" hide-center-plus>
        <div
          class="absolute top-10 md:top-4 left-4 text-[10px] md:text-[11px] tracking-widest uppercase font-medium text-neutral-600"
        >
          <span class="md:hidden">IoT Eng / AI Eng</span>
          <span class="hidden md:inline">IoT Engineer / Ai Engineer</span>
        </div>

        <div
          class="absolute bottom-6 md:bottom-auto md:top-4 left-4 md:left-auto md:right-4 text-[10px] md:text-[11px] tracking-wider font-medium text-neutral-600 text-left md:text-right"
        >
          fadhlurrohman1204@gmail.com
        </div>

        <div
          class="absolute top-4 md:top-[calc(50%+0.5rem)] left-4 text-[11px] tracking-widest uppercase font-medium text-neutral-600"
        >
          Fadhlur Rohman
        </div>

        <div
          class="absolute bottom-6 md:bottom-auto md:top-[calc(50%+0.5rem)] right-4 md:right-4 text-[10px] md:text-[11px] tracking-widest uppercase font-medium text-neutral-600 text-right"
        >
          @2026
        </div>
      </BlueprintGrid>
    </div>
  </section>
</template>

<script setup>
import BlueprintGrid from '../ui/BlueprintGrid.vue'
import BlueprintRuler from '../ui/BlueprintRuler.vue'
</script>

<style scoped>
.font-serif {
  font-family:
    Garamond, Baskerville, 'Baskerville Old Face', 'Hoefler Text', 'Times New Roman', serif;
}
</style>
