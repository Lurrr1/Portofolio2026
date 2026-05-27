<template>
  <section
    class="relative w-full min-h-screen md:h-screen bg-[#ebebeb] text-[#1a1a1a] font-sans md:overflow-hidden select-none py-12 md:py-0"
  >
    <BlueprintRuler position="top" :marker-index="60" class="z-50" />
    <BlueprintRuler position="bottom" :marker-index="90" class="z-50" />

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-20">
      <BlueprintGrid :rows="3" :cols="5" :white-markers="[]" :black-markers="[1, 6, 11]" />
    </div>

    <div
      class="relative md:absolute md:inset-0 m-4 md:m-8 p-6 md:p-0 flex flex-col md:flex-row gap-8 md:gap-0 pointer-events-auto"
    >
      <div
        class="w-full md:w-1/2 h-auto md:h-full flex flex-col gap-6 md:gap-0 relative z-30 px-0 md:px-6 py-8 md:py-12 lg:p-12"
      >
        <div class="relative w-full h-auto md:h-1/2 flex flex-col justify-center">
          <div
            class="md:hidden text-[11px] font-bold tracking-widest text-neutral-900 mb-2 mt-4 md:mt-0"
          >
            02
          </div>

          <div
            class="md:hidden text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 mb-2"
          >
            Research & Deep Learning
          </div>

          <div
            class="hidden md:block absolute top-4 left-6 text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 z-50"
          >
            Research & Deep Learning
          </div>

          <div class="mt-0 md:mt-4 md:pl-6 lg:pl-10">
            <h2
              class="text-[2.5rem] md:text-4xl lg:text-[3.5rem] font-serif leading-[1] md:leading-[1.05] tracking-tight text-neutral-900 mb-4 md:mb-6 pr-4 mt-0"
            >
              PM 2.5 Carbon Concentration Detection
            </h2>
            <p
              class="text-[11px] lg:text-[13px] text-neutral-700 leading-relaxed font-medium max-w-md"
            >
              This research addresses the critical challenge of detecting and analyzing carbon
              concentration at the PM 2.5 scale across Indonesia and Malaysia. By combining
              Terahertz (THz) sensing technology with a Convolutional Neural Network (CNN) trained
              on MODIS satellite data, the intelligent system achieved an average accuracy of 93.4%
              and an F1-score of 92.9% for forest fire hotspot detection.
            </p>
          </div>
        </div>

        <div class="relative w-full h-auto md:h-1/2 flex flex-col justify-center mt-6 md:mt-0">
          <div class="flex flex-col gap-4 md:gap-5 w-full max-w-md md:pl-6 lg:pl-10">
            <div class="flex flex-col sm:flex-row items-start gap-1 sm:gap-0">
              <div
                class="text-[11px] font-bold uppercase tracking-widest text-neutral-900 w-full sm:w-28 lg:w-36 shrink-0 sm:pt-0.5"
              >
                Symposium
              </div>
              <div class="flex-1">
                <p class="text-[12px] font-bold text-neutral-900 leading-none">
                  28th CEReS Symposium
                </p>
                <p class="text-[11px] text-neutral-600 mt-1.5 leading-relaxed">
                  Chiba University, Japan (Nov 30 - Dec 1, 2025)
                </p>
              </div>
            </div>

            <div class="flex flex-col sm:flex-row items-start gap-1 sm:gap-0">
              <div
                class="text-[11px] font-bold uppercase tracking-widest text-neutral-900 w-full sm:w-28 lg:w-36 shrink-0 sm:pt-0.5"
              >
                Tech Stack
              </div>
              <div class="flex-1">
                <p class="text-[12px] font-bold text-neutral-900 leading-none">
                  Deep Learning & Cloud Computing
                </p>
                <p class="text-[11px] text-neutral-600 mt-1.5 leading-relaxed">
                  CNN Algorithm, THz Sensing, MODIS Satellite Data
                </p>
              </div>
            </div>

            <div class="flex flex-col sm:flex-row items-start gap-1 sm:gap-0">
              <div
                class="text-[11px] font-bold uppercase tracking-widest text-neutral-900 w-full sm:w-28 lg:w-36 shrink-0 sm:pt-0.5"
              >
                Role
              </div>
              <div class="flex-1">
                <p class="text-[12px] font-bold text-neutral-900 leading-none">
                  Co-Author & Research Assistant
                </p>
                <p class="text-[11px] text-neutral-600 mt-1.5 leading-relaxed">
                  Universitas Islam Riau
                </p>
              </div>
            </div>

            <div class="flex flex-col sm:flex-row items-start gap-1 sm:gap-0">
              <div
                class="text-[11px] font-bold uppercase tracking-widest text-neutral-900 w-full sm:w-28 lg:w-36 shrink-0 sm:pt-0.5"
              >
                Co-Authors
              </div>
              <div class="flex-1">
                <p class="text-[12px] font-bold text-neutral-900 leading-none">Research Team</p>
                <p class="text-[11px] text-neutral-600 mt-1.5 leading-relaxed">
                  Evizal Abdul Kadir, Hitoshi Irie, Sri Listia Rosa
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div
        class="w-full md:w-1/2 h-auto md:h-full flex items-center justify-center relative mt-8 md:mt-0 z-10 mb-12 md:mb-0"
      >
        <div
          class="hidden md:block absolute top-4 right-6 text-[11px] font-bold tracking-widest text-neutral-900 mix-blend-difference pointer-events-none z-50"
        >
          02
        </div>

        <div
          class="w-[85%] sm:w-[60%] md:w-auto md:h-[75%] lg:h-[80%] aspect-[1/1.414] bg-neutral-300 rounded-sm overflow-hidden shadow-2xl group relative ring-1 ring-neutral-400/50 cursor-pointer pointer-events-auto"
        >
          <img
            src="../../../public/images/Sensing.webp"
            alt="Environmental Remote Sensing Poster"
            class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
          />
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
