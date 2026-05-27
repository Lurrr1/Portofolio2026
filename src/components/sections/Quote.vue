<template>
  <section
    class="relative w-full h-auto md:h-screen bg-[#ebebeb] text-[#1a1a1a] font-sans md:overflow-hidden select-none flex items-center justify-center py-16 md:py-0"
  >
    <BlueprintRuler position="top" :marker-index="50" class="z-50" />
    <BlueprintRuler position="bottom" :marker-index="90" class="z-50" />

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-20">
      <BlueprintGrid :rows="3" :cols="5" />
    </div>

    <div class="relative md:absolute md:inset-0 m-4 md:m-8 flex flex-col pointer-events-auto">
      <div class="md:hidden absolute top-10 left-6 flex flex-col z-30">
        <div class="text-[11px] font-bold tracking-widest text-neutral-900 mb-1">07</div>
        <div class="text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500">
          Education & Mentorship
        </div>
      </div>

      <div
        class="hidden md:block absolute top-14 left-6 text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 z-30"
      >
        Education & Mentorship
      </div>
      <div
        class="hidden md:block absolute top-14 right-6 text-[11px] font-bold tracking-widest text-neutral-900 z-30"
      >
        07
      </div>

      <div
        class="w-full h-auto md:h-1/2 flex items-center justify-center relative px-6 md:px-0 pt-28 pb-12 md:py-0 z-30"
      >
        <h2
          class="w-full md:w-[90vw] lg:w-[85vw] max-w-[1300px] text-[1.75rem] leading-tight md:text-4xl lg:text-[3.2rem] font-serif md:leading-[1.05] tracking-tight text-neutral-900 text-center mix-blend-multiply pointer-events-none"
        >
          Mentoring the community to bridge the gap between theoretical knowledge and practical
          hardware implementation in end-to-end IoT solutions.
        </h2>
      </div>

      <div
        class="w-full h-auto md:h-1/2 grid grid-cols-2 md:flex relative z-10 gap-2 md:gap-0 px-6 md:px-0 pb-8 md:pb-2 lg:pb-3 md:pt-4 lg:pt-6"
      >
        <div class="w-full md:w-1/4 h-full aspect-square md:aspect-auto relative md:pr-1.5">
          <div
            class="w-full h-full bg-neutral-300 rounded-sm overflow-hidden shadow-md transition-all duration-700 group cursor-pointer ring-1 ring-neutral-400/50"
          >
            <img
              src="D:\Vue\Porto\public\images\Asdos.webp"
              alt="Teaching Assistantship"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>
        </div>

        <div class="w-full md:w-1/4 h-full aspect-square md:aspect-auto relative md:px-1.5">
          <div
            class="w-full h-full bg-neutral-300 rounded-sm overflow-hidden shadow-md transition-all duration-700 group cursor-pointer ring-1 ring-neutral-400/50"
          >
            <img
              src="D:\Vue\Porto\public\images\Organisasi.webp"
              alt="Organizational Mentorship"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>
        </div>

        <div class="w-full md:w-1/4 h-full aspect-square md:aspect-auto relative md:px-1.5">
          <div
            class="w-full h-full bg-neutral-300 rounded-sm overflow-hidden shadow-md transition-all duration-700 group cursor-pointer ring-1 ring-neutral-400/50"
          >
            <img
              src="D:\Vue\Porto\public\images\Organisasi1.webp"
              alt="Project Mentorship"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>
        </div>

        <div class="w-full md:w-1/4 h-full aspect-square md:aspect-auto relative md:pl-1.5">
          <div
            class="w-full h-full bg-neutral-300 rounded-sm overflow-hidden shadow-md transition-all duration-700 group cursor-pointer ring-1 ring-neutral-400/50"
          >
            <img
              src="D:\Vue\Porto\public\images\Sd.webp"
              alt="Community Mentorship"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>
        </div>
      </div>
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
