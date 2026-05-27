<template>
  <section
    class="relative w-full min-h-screen md:h-screen bg-[#ebebeb] text-[#1a1a1a] font-sans md:overflow-hidden select-none py-24 md:py-0"
  >
    <BlueprintRuler position="top" :marker-index="10" />
    <BlueprintRuler position="bottom" :marker-index="60" />

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-10">
      <BlueprintGrid :rows="2" :cols="5" />
    </div>

    <div
      class="relative md:absolute md:inset-0 m-4 md:m-8 p-6 md:p-8 lg:p-12 flex flex-col md:flex-row gap-12 md:gap-8 lg:gap-16 z-20"
    >
      <div
        class="hidden md:block absolute top-4 right-6 text-[11px] font-bold tracking-widest text-neutral-900 z-30"
      >
        01
      </div>

      <div class="w-full md:w-1/2 flex flex-col justify-between h-auto md:h-full gap-8 md:gap-0">
        <div class="relative">
          <div class="md:hidden text-[11px] font-bold tracking-widest text-neutral-900 mb-4">
            01
          </div>
          <h2
            class="text-3xl lg:text-[2.75rem] font-serif leading-[1.05] tracking-tight text-neutral-900"
          >
            I build end-to-end systems that are consistent, intentional, and thoughtfully
            structured.
          </h2>
        </div>

        <div class="flex flex-col md:flex-row gap-6 mt-4 md:mt-8 h-auto md:h-full min-h-0">
          <div
            class="w-full md:w-[45%] flex flex-row md:flex-col justify-between items-center md:items-start gap-4 md:gap-0"
          >
            <div
              class="w-28 md:w-full h-28 md:h-40 lg:h-64 bg-neutral-300 overflow-hidden rounded-sm shrink-0 shadow-md"
            >
              <img
                src="/images/Profil.webp"
                alt="Fadhlur Rohman"
                class="w-full h-full object-cover hover:scale-105 transition-transform duration-700"
              />
            </div>

            <div class="mt-0 md:mt-4 mb-2">
              <h3 class="text-[10px] font-bold uppercase tracking-widest text-neutral-900 mb-1">
                Contact
              </h3>
              <p
                class="text-[11px] text-neutral-600 font-medium leading-tight whitespace-normal md:whitespace-nowrap"
              >
                fadhlurrohman1204@gmail.com
              </p>
            </div>
          </div>

          <div
            class="w-full md:w-[55%] flex flex-col gap-4 text-[11px] lg:text-[13px] text-neutral-700 leading-relaxed font-medium md:overflow-y-auto hide-scrollbar md:pr-2 md:pl-4 lg:pl-8"
          >
            <p>
              I'm Fadhlur Rohman, an IoT Engineer and Machine Learning Specialist exploring the
              intersection of hardware and artificial intelligence.
            </p>
            <p>
              Currently based in Dumai, Riau, Indonesia, my work focuses on building seamless
              connections between physical devices and data-driven insights. From developing
              empathetic virtual assistants to implementing CNN algorithms for environmental
              monitoring, I ensure data reliability.
            </p>
            <p>
              I work across embedded systems (ESP32, C++), software development, and deep learning,
              creating technology that is both strategic and impactful for the community.
            </p>
          </div>
        </div>
      </div>

      <div
        class="w-full md:w-1/2 flex flex-col justify-between h-auto md:h-full pt-8 md:pt-2 md:pl-10 lg:pl-16 border-t border-neutral-300/40 md:border-none"
      >
        <div class="flex flex-col gap-8 w-full lg:ml-[150px]">
          <div>
            <h3
              class="text-[11px] font-bold underline underline-offset-4 mb-6 uppercase tracking-widest text-neutral-900"
            >
              Education
            </h3>

            <div class="flex flex-col sm:flex-row items-start mb-5 gap-1 sm:gap-0">
              <div
                class="text-[11px] text-neutral-500 w-full sm:w-28 lg:w-36 shrink-0 font-medium tracking-wider pt-0.5"
              >
                2022 - 2026
              </div>
              <div class="flex-1">
                <p class="text-[13px] font-bold text-neutral-900 leading-none">
                  Universitas Islam Riau
                </p>
                <p class="text-[11px] text-neutral-600 mt-1.5 leading-relaxed">
                  Bachelor of Computer Engineering Technology
                </p>
              </div>
            </div>

            <div class="flex flex-col sm:flex-row items-start mb-5 gap-1 sm:gap-0">
              <div
                class="text-[11px] text-neutral-500 w-full sm:w-28 lg:w-36 shrink-0 font-medium tracking-wider pt-0.5"
              >
                2024 - 2025
              </div>
              <div class="flex-1">
                <p class="text-[13px] font-bold text-neutral-900 leading-none">Bangkit Academy</p>
                <p class="text-[11px] text-neutral-600 mt-1.5 leading-relaxed">
                  Machine Learning Cohort
                </p>
              </div>
            </div>
          </div>

          <div>
            <h3
              class="text-[11px] font-bold underline underline-offset-4 mb-6 uppercase tracking-widest text-neutral-900"
            >
              Experience
            </h3>

            <div class="flex flex-col sm:flex-row items-start mb-5 gap-1 sm:gap-0">
              <div
                class="text-[11px] text-neutral-500 w-full sm:w-28 lg:w-36 shrink-0 font-medium tracking-wider pt-0.5"
              >
                10/25 - 12/25
              </div>
              <div class="flex-1">
                <p class="text-[13px] font-bold text-neutral-900 leading-none">
                  Research Assistant
                </p>
                <p class="text-[11px] text-neutral-600 mt-1.5 leading-relaxed">
                  CERES Symposium & UIR
                </p>
              </div>
            </div>

            <div class="flex flex-col sm:flex-row items-start mb-5 gap-1 sm:gap-0">
              <div
                class="text-[11px] text-neutral-500 w-full sm:w-28 lg:w-36 shrink-0 font-medium tracking-wider pt-0.5"
              >
                09/24 - 09/25
              </div>
              <div class="flex-1">
                <p class="text-[13px] font-bold text-neutral-900 leading-none">Chairman</p>
                <p class="text-[11px] text-neutral-600 mt-1.5 leading-relaxed">
                  Groot UIR Robotic and Automation
                </p>
              </div>
            </div>

            <div class="flex flex-col sm:flex-row items-start mb-5 gap-1 sm:gap-0">
              <div
                class="text-[11px] text-neutral-500 w-full sm:w-28 lg:w-36 shrink-0 font-medium tracking-wider pt-0.5"
              >
                10/25 - 12/25
              </div>
              <div class="flex-1">
                <p class="text-[13px] font-bold text-neutral-900 leading-none">
                  IoT Teaching Assistant
                </p>
                <p class="text-[11px] text-neutral-600 mt-1.5 leading-relaxed">
                  Universitas Islam Riau
                </p>
              </div>
            </div>
          </div>
        </div>

        <div class="mt-12 md:mt-auto pt-4 md:pl-2">
          <h2
            class="text-2xl lg:text-3xl font-serif leading-[1.1] tracking-tight text-neutral-900 pr-4"
          >
            I appreciate reliable systems where logic, hardware, and data come together.
          </h2>
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

.hide-scrollbar::-webkit-scrollbar {
  display: none;
}
.hide-scrollbar {
  -ms-overflow-style: none;
  scrollbar-width: none;
}
</style>
