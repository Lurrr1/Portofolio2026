<template>
  <section
    class="relative w-full min-h-screen md:h-screen bg-[#ebebeb] text-[#1a1a1a] font-sans md:overflow-hidden select-none py-12 md:py-0"
  >
    <BlueprintRuler position="top" :marker-index="60" class="z-50" />
    <BlueprintRuler position="bottom" :marker-index="100" class="z-50" />

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-20">
      <BlueprintGrid
        :rows="3"
        :cols="5"
        :white-markers="[8]"
        :black-markers="[0, 1, 2, 3, 5, 6, 7, 8, 10, 11, 12, 13]"
      />
    </div>

    <div
      class="relative md:absolute md:inset-0 m-4 md:m-8 p-6 md:p-0 flex flex-col md:flex-row gap-10 md:gap-0"
    >
      <div
        class="w-full md:w-1/2 h-auto md:h-full flex flex-col justify-between md:p-8 lg:p-12 relative md:border-r border-neutral-300/30 z-30"
      >
        <div class="md:hidden text-[11px] font-bold tracking-widest text-neutral-900 mb-2">04</div>

        <div
          class="md:hidden text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 mb-2"
        >
          Leadership
        </div>
        <div
          class="hidden md:block absolute top-4 left-6 text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 z-50"
        >
          Leadership
        </div>

        <div class="mt-2 md:mt-8 lg:mt-12">
          <h2
            class="text-5xl lg:text-[4.5rem] font-serif leading-[0.95] tracking-tight text-neutral-900 mb-6 md:mb-8"
          >
            Chairman.
          </h2>

          <ul
            class="text-[11px] lg:text-[13px] text-neutral-700 leading-relaxed font-medium list-disc pl-4 space-y-3 max-w-md pr-2"
          >
            <li>
              Led the university’s primary robotics and automation student organization, overseeing
              technical development and member training.
            </li>
            <li>
              Orchestrated various technical workshops and seminars focused on IoT and embedded
              systems to enhance member skillsets.
            </li>
            <li>
              Managed strategic organizational planning, including partnership coordination and
              representing the group in university-level forums.
            </li>
          </ul>
        </div>

        <div class="mt-8 md:mt-auto pt-4 md:pt-12 pb-4 flex flex-col gap-2.5">
          <div class="flex items-start">
            <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">
              Organization
            </div>
            <div class="text-[11px] text-neutral-700 font-medium leading-tight">
              Groot UIR Robotic and Automation
            </div>
          </div>
          <div class="flex items-start">
            <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">Period</div>
            <div class="text-[11px] text-neutral-700 font-medium leading-tight">
              09/2024 - 09/2025
            </div>
          </div>
          <div class="flex items-start">
            <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">Location</div>
            <div class="text-[11px] text-neutral-700 font-medium leading-tight">Pekanbaru</div>
          </div>
        </div>
      </div>

      <div
        class="w-full md:w-1/2 h-auto md:h-full flex items-center justify-center md:justify-end relative pointer-events-auto mt-4 md:mt-0 z-10"
      >
        <div
          class="hidden md:block absolute top-4 right-6 text-[11px] font-bold tracking-widest text-black z-50 mix-blend-difference pointer-events-none"
        >
          04
        </div>

        <div
          class="w-full aspect-[25/18] md:max-h-[75%] lg:max-h-[80%] bg-neutral-300 overflow-hidden shadow-2xl ring-1 ring-neutral-400/50 flex flex-col gap-0 z-10"
        >
          <div class="w-full h-1/2 grid grid-cols-[9fr_16fr] gap-0">
            <div
              class="overflow-hidden relative group cursor-pointer border-r border-neutral-100/20"
            >
              <img
                src="../../../public/images/Me.webp"
                alt="Groot 1:1 Top"
                class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
              />
            </div>
            <div
              class="overflow-hidden relative group cursor-pointer border-b border-neutral-100/20"
            >
              <img
                src="../../../public/images/Groot.webp"
                alt="Groot 16:9 Atas"
                class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
              />
            </div>
          </div>

          <div class="w-full h-1/2 grid grid-cols-[16fr_9fr] gap-0">
            <div
              class="overflow-hidden relative group cursor-pointer border-r border-neutral-100/20"
            >
              <img
                src="../../../public/images/Groot2.webp"
                alt="Groot 16:9 Bawah"
                class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
              />
            </div>
            <div class="overflow-hidden relative group cursor-pointer">
              <img
                src="../../../public/images/Chairman.webp"
                alt="Chairman"
                class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
              />
            </div>
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
