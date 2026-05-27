<template>
  <section
    class="relative w-full h-auto md:h-screen bg-[#ebebeb] text-[#1a1a1a] font-sans md:overflow-hidden select-none py-16 md:py-0"
  >
    <BlueprintRuler position="top" :marker-index="90" class="z-50" />
    <BlueprintRuler position="bottom" :marker-index="20" class="z-50" />

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-20">
      <BlueprintGrid
        :rows="3"
        :cols="5"
        :white-markers="[7, 8, 9]"
        :black-markers="[0, 1, 2, 5, 6, 10, 11, 12]"
      />
    </div>

    <div
      class="relative md:absolute md:inset-0 m-4 md:m-8 p-6 md:p-0 flex flex-col md:flex-row gap-10 md:gap-0"
    >
      <div class="w-full md:w-1/2 h-auto md:h-full flex flex-col md:p-8 lg:p-12 relative z-30 mt-0">
        <div class="md:hidden flex flex-col mb-2">
          <div class="text-[11px] font-bold tracking-widest text-neutral-900 mb-1">08</div>
          <div class="text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500">
            Competitions & Mentorship
          </div>
        </div>

        <div
          class="hidden md:block absolute top-4 left-6 text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500"
        >
          Competitions
        </div>

        <div class="mt-2 md:mt-8 mb-6 md:mb-8 shrink-0">
          <h2
            class="text-[2.5rem] md:text-4xl lg:text-[3.5rem] font-serif leading-[1] tracking-tight text-neutral-900"
          >
            Beyond the<br />Classroom
          </h2>
        </div>

        <div
          ref="scrollContainer"
          @mouseenter="startAutoScroll"
          @mouseleave="stopAutoScroll"
          @wheel="stopAutoScroll"
          class="flex-none md:flex-1 overflow-visible md:overflow-y-auto hide-scrollbar pr-0 md:pr-6 space-y-6 md:space-y-8 pb-0 md:pb-10 pointer-events-auto"
        >
          <div class="flex flex-col gap-1.5">
            <h3
              class="text-[13px] lg:text-[14px] font-bold uppercase tracking-widest text-neutral-900"
            >
              Technical Mentor
            </h3>
            <p class="text-[11px] font-bold text-neutral-500 mb-2 tracking-wider">
              Pekan Elektro 2025
            </p>
            <ul
              class="text-[11px] lg:text-[12px] text-neutral-700 leading-relaxed font-medium list-disc pl-4 space-y-2"
            >
              <li>
                Acted as a technical advisor and coach for junior student teams competing in
                national-level electrical and robotics challenges.
              </li>
              <li>
                Provided guidance on systems integration and competition strategy, fostering the
                team's technical proficiency and problem-solving skills.
              </li>
            </ul>
          </div>

          <div class="flex flex-col gap-1.5">
            <h3
              class="text-[13px] lg:text-[14px] font-bold uppercase tracking-widest text-neutral-900"
            >
              Hackathon Participant <span class="text-neutral-500 font-normal">(Team Echo)</span>
            </h3>
            <p class="text-[11px] font-bold text-neutral-500 mb-2 tracking-wider">
              HackFest 2024 Google Developer Student Clubs (GDSC)
            </p>
            <ul
              class="text-[11px] lg:text-[12px] text-neutral-700 leading-relaxed font-medium list-disc pl-4 space-y-2"
            >
              <li>
                Participated in a national hackathon to build a technology solution addressing the
                United Nations' 17 Sustainable Development Goals (SDGs).
              </li>
              <li>
                Developed AgroSmart utilizing ESP32, Firebase, and Flutter for Agriculture
                Automation.
              </li>
              <li>
                Designed the firmware architecture using C++ for ESP32 and integrated IoT sensor
                data with Firebase for real-time agricultural monitoring.
              </li>
            </ul>
          </div>

          <div class="flex flex-col gap-1.5">
            <h3
              class="text-[13px] lg:text-[14px] font-bold uppercase tracking-widest text-neutral-900"
            >
              Competitive Programmer
            </h3>
            <p class="text-[11px] font-bold text-neutral-500 mb-2 tracking-wider">i-CPROM 2023</p>
            <ul
              class="text-[11px] lg:text-[12px] text-neutral-700 leading-relaxed font-medium list-disc pl-4 space-y-2"
            >
              <li>
                Represented Universitas Islam Riau in the International Competitive Programming and
                Multimedia Competition (i-CPROM 2023).
              </li>
              <li>
                Competed in the Programming Competition category, collaborating in a 3-person team
                to solve algorithmic and logical challenges under time pressure.
              </li>
              <li>
                Mentored by Dr. Apri Siswanto to develop efficient algorithms and problem-solving
                strategies.
              </li>
            </ul>
          </div>
        </div>
      </div>

      <div
        class="w-full md:w-1/2 h-auto md:h-full relative flex items-center justify-center md:justify-start pointer-events-auto mt-4 md:mt-0 mb-8 md:mb-0 z-10"
      >
        <div
          class="hidden md:block absolute top-4 right-6 text-[11px] font-bold tracking-widest text-black mix-blend-difference z-50 pointer-events-none"
        >
          08
        </div>

        <div
          class="w-full md:w-[calc(100%+2rem)] h-auto md:h-[85%] lg:h-[90%] grid grid-cols-2 md:grid-cols-3 md:grid-rows-3 gap-0 md:rounded-l-sm overflow-hidden shadow-2xl ring-1 ring-neutral-400/50"
        >
          <div
            class="col-span-2 md:col-start-2 md:row-start-1 md:col-span-2 md:row-span-2 bg-neutral-300 overflow-hidden cursor-pointer group relative aspect-video md:aspect-auto border-b md:border-b-0 border-neutral-100/20"
          >
            <img
              src="../../../public/images/Electro.webp"
              alt="Electronics Team"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>

          <div
            class="col-span-1 md:col-start-1 md:row-start-1 bg-neutral-300 overflow-hidden cursor-pointer group relative aspect-square md:aspect-auto border-b border-r md:border-b-0 md:border-r-0 border-neutral-100/20"
          >
            <img
              src="../../../public/images/Cprom.webp"
              alt="Cprom"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>

          <div
            class="col-span-1 md:col-start-1 md:row-start-2 md:row-span-2 bg-neutral-300 overflow-hidden cursor-pointer group relative aspect-square md:aspect-auto border-b md:border-b-0 border-neutral-100/20"
          >
            <img
              src="../../../public/images/Agrosmart.webp"
              alt="AgroSmart"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>

          <div
            class="col-span-1 md:col-start-2 md:row-start-3 bg-neutral-300 overflow-hidden cursor-pointer group relative aspect-square md:aspect-auto border-r md:border-r-0 border-neutral-100/20"
          >
            <img
              src="../../../public/images/Echo.webp"
              alt="Echo"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>

          <div
            class="col-span-1 md:col-start-3 md:row-start-3 bg-neutral-300 overflow-hidden cursor-pointer group relative aspect-square md:aspect-auto"
          >
            <img
              src="../../../public/images/Bangkit.webp"
              alt="Bangkit"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'
import BlueprintGrid from '../ui/BlueprintGrid.vue'
import BlueprintRuler from '../ui/BlueprintRuler.vue'

// Logika Auto-Scroll (Hanya aktif di Desktop)
const scrollContainer = ref(null)
let scrollInterval = null
let isScrollingDown = true

const startAutoScroll = () => {
  if (window.innerWidth < 768) return

  stopAutoScroll()

  scrollInterval = setInterval(() => {
    if (!scrollContainer.value) return

    const el = scrollContainer.value

    if (el.scrollTop + el.clientHeight >= el.scrollHeight - 1) {
      isScrollingDown = false
    } else if (el.scrollTop <= 0) {
      isScrollingDown = true
    }

    el.scrollTop += isScrollingDown ? 1 : -1
  }, 40)
}

const stopAutoScroll = () => {
  if (scrollInterval) {
    clearInterval(scrollInterval)
    scrollInterval = null
  }
}
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
