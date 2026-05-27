<template>
  <section
    class="relative w-full min-h-screen md:h-screen bg-[#ebebeb] text-[#1a1a1a] font-sans md:overflow-hidden select-none py-12 md:py-0"
  >
    <BlueprintRuler position="top" :marker-index="100" class="z-50" />
    <BlueprintRuler position="bottom" :marker-index="20" class="z-50" />

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-20">
      <BlueprintGrid
        :rows="3"
        :cols="5"
        :white-markers="[6]"
        :black-markers="[0, 1, 2, 5, 6, 10, 11, 12]"
      />
    </div>

    <div
      class="relative md:absolute md:inset-0 m-4 md:m-8 p-6 md:p-0 flex flex-col md:flex-row gap-10 md:gap-0 pointer-events-auto"
    >
      <div
        class="w-full md:w-1/2 h-auto md:h-full flex flex-col justify-between p-0 md:p-8 lg:p-12 md:border-r border-neutral-300/40 relative"
      >
        <div class="relative z-30">
          <div class="md:hidden text-[11px] font-bold tracking-widest text-neutral-900 mb-2">
            05
          </div>

          <div
            class="text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 mb-4 md:mb-6 mt-2 md:mt-0"
          >
            Academic Leadership
          </div>
          <h2
            class="text-[2.5rem] md:text-4xl lg:text-[3.5rem] font-serif leading-[1] md:leading-[1.0] tracking-tight text-neutral-900 mb-4 md:mb-6 pr-4"
          >
            Teaching &<br />Community.
          </h2>
          <p
            class="text-[12px] lg:text-[13px] text-neutral-700 leading-relaxed font-medium max-w-sm"
          >
            Bridging the gap between theoretical knowledge and real-world impact through technical
            mentorship and IoT-driven community service.
          </p>
        </div>

        <div
          class="w-full aspect-video bg-neutral-300 rounded-sm overflow-hidden shadow-lg transition-all duration-700 ring-1 ring-neutral-400/50 mt-8 md:mt-auto group cursor-pointer relative z-10"
        >
          <img
            src="D:\Vue\Porto\public\images\Comunity.webp"
            alt="IoT Teaching and Community Service"
            class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
          />
        </div>
      </div>

      <div
        class="w-full md:w-1/2 h-auto md:h-full flex flex-col justify-center p-0 md:px-8 lg:px-16 py-0 md:py-8 relative z-30 mt-4 md:mt-0"
      >
        <div
          class="hidden md:block absolute top-4 right-6 text-[11px] font-bold tracking-widest text-neutral-900 z-50"
        >
          05
        </div>

        <div class="flex flex-col justify-center gap-8 lg:gap-12 w-full mt-4 md:mt-0">
          <div
            class="flex flex-col justify-center relative py-4 md:py-6 border-b border-neutral-300/50 group"
          >
            <div
              class="hidden xl:block absolute top-6 left-0 text-[10px] font-bold tracking-widest text-neutral-400 -translate-x-[4.5rem]"
            >
              2025
            </div>

            <div class="flex flex-col md:flex-row gap-4 md:gap-8 items-start">
              <div class="w-full md:w-[35%] shrink-0">
                <h3 class="text-[13px] font-bold text-neutral-900 leading-tight">
                  Teaching Assistant
                </h3>
                <span class="text-neutral-500 font-medium text-[11px] tracking-wide mt-1 block">
                  Community Service
                </span>
                <span
                  class="xl:hidden text-neutral-400 font-bold text-[10px] tracking-widest mt-2 block"
                >
                  2025
                </span>
              </div>

              <div class="flex-1 space-y-3">
                <p
                  class="text-[11px] lg:text-[11.5px] text-neutral-700 leading-relaxed font-medium"
                >
                  Collaborated with university faculty (led by Assoc. Prof. Dr. Ir. Evizal) on the
                  initiative: "Implementation of Siak River Water Quality Monitoring System and
                  Clean Water Distillation."
                </p>
                <p
                  class="text-[11px] lg:text-[11.5px] text-neutral-700 leading-relaxed font-medium"
                >
                  Deployed IoT-based sensor devices to monitor water temperature, pH, turbidity, and
                  electrical conductivity in real-time, integrating data transmission directly to
                  cloud servers for web and mobile access.
                </p>
                <p
                  class="text-[11px] lg:text-[11.5px] text-neutral-700 leading-relaxed font-medium"
                >
                  Assisted in the installation of a multi-stage clean water distillation unit
                  (mechanical filtration, active carbon, RO, and UV) that successfully met the
                  Indonesian Ministry of Health standards.
                </p>
              </div>
            </div>
          </div>

          <div class="flex flex-col justify-center relative py-4 md:py-6 group">
            <div
              class="hidden xl:block absolute top-6 left-0 text-[10px] font-bold tracking-widest text-neutral-400 -translate-x-[4.5rem]"
            >
              2025
            </div>

            <div class="flex flex-col md:flex-row gap-4 md:gap-8 items-start">
              <div class="w-full md:w-[35%] shrink-0">
                <h3 class="text-[13px] font-bold text-neutral-900 leading-tight">
                  Teaching Assistant
                </h3>
                <span class="text-neutral-500 font-medium text-[11px] tracking-wide mt-1 block">
                  Internet of Things (IoT)
                </span>
                <span
                  class="xl:hidden text-neutral-400 font-bold text-[10px] tracking-widest mt-2 block"
                >
                  2025
                </span>
              </div>

              <div class="flex-1 space-y-3">
                <p
                  class="text-[11px] lg:text-[11.5px] text-neutral-700 leading-relaxed font-medium"
                >
                  Assisted the primary lecturer in delivering comprehensive IoT course materials and
                  guiding students through practical laboratory sessions.
                </p>
                <p
                  class="text-[11px] lg:text-[11.5px] text-neutral-700 leading-relaxed font-medium"
                >
                  Mentored students in developing hardware projects using microcontrollers and
                  sensor integration, ensuring strong foundational knowledge in embedded systems.
                </p>
              </div>
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
