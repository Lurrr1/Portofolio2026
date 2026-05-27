<template>
  <section
    class="relative w-full min-h-screen md:h-screen bg-[#ebebeb] text-[#1a1a1a] font-sans md:overflow-hidden select-none py-12 md:py-0"
  >
    <BlueprintRuler position="top" :marker-index="90" class="z-50" />
    <BlueprintRuler position="bottom" :marker-index="60" class="z-50" />

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-20">
      <BlueprintGrid
        :rows="3"
        :cols="5"
        :white-markers="[1, 6, 11]"
        :black-markers="[2, 3, 4, 7, 8, 9, 12, 13, 14]"
      />
    </div>

    <div
      class="relative md:absolute md:inset-0 m-4 md:m-8 p-6 md:p-0 flex flex-col md:flex-row gap-6 md:gap-0"
    >
      <div class="md:hidden flex flex-col w-full z-30 mb-2">
        <div class="text-[11px] font-bold tracking-widest text-neutral-900 mb-3">03</div>
        <div class="text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 mb-2">
          Machine Learning
        </div>
        <h2 class="text-[2.5rem] font-serif leading-[1.05] tracking-tight text-neutral-900">
          Bangkit<br />Academy.
        </h2>
      </div>

      <div
        class="w-full md:w-1/2 h-auto md:h-full flex flex-col justify-center items-start md:items-center relative pointer-events-auto z-10"
      >
        <div
          class="hidden md:block absolute top-4 left-6 text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 z-30"
        >
          Machine Learning
        </div>

        <div
          class="w-full aspect-square md:aspect-auto md:w-full md:h-[75%] lg:h-[80%] bg-neutral-300 overflow-hidden shadow-xl ring-1 ring-neutral-400/50 mt-2 md:mt-0"
        >
          <div class="w-full h-full flex gap-0">
            <div class="w-[35%] h-full flex flex-col gap-0">
              <div
                class="h-[40%] w-full bg-neutral-400 overflow-hidden group cursor-pointer relative"
              >
                <img
                  src="D:\Vue\Porto\public\images\Team1.webp"
                  alt="Team 1"
                  class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
                />
              </div>

              <div
                class="h-[60%] w-full bg-neutral-400 overflow-hidden group cursor-pointer relative"
              >
                <img
                  src="D:\Vue\Porto\public\images\View.webp"
                  alt="View"
                  class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
                />
              </div>
            </div>

            <div class="w-[65%] h-full flex flex-col gap-0">
              <div
                class="h-[60%] w-full bg-neutral-400 overflow-hidden group cursor-pointer relative"
              >
                <img
                  src="D:\Vue\Porto\public\images\Final.webp"
                  alt="Final"
                  class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
                />
              </div>

              <div class="h-[40%] w-full flex gap-0">
                <div
                  class="w-[45%] h-full bg-neutral-400 overflow-hidden group cursor-pointer relative"
                >
                  <img
                    src="D:\Vue\Porto\public\images\Team.webp"
                    alt="Team"
                    class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
                  />
                </div>

                <div
                  class="w-[55%] h-full bg-neutral-400 overflow-hidden group cursor-pointer relative"
                >
                  <img
                    src="D:\Vue\Porto\public\images\Glusity.webp"
                    alt="Glusity"
                    class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div
        class="w-full md:w-1/2 h-auto md:h-full flex flex-col justify-center p-0 md:p-8 lg:p-12 relative z-30 md:border-l border-neutral-300/30 mt-6 md:mt-0"
      >
        <div
          class="hidden md:block absolute top-4 right-6 text-[11px] font-bold tracking-widest text-neutral-900"
        >
          03
        </div>

        <div class="md:pl-[50px] lg:pl-[100px]">
          <h2
            class="hidden md:block text-5xl lg:text-[4rem] font-serif leading-[0.95] tracking-tight text-neutral-900 mb-8"
          >
            Bangkit<br />Academy.
          </h2>

          <ul
            class="text-[11px] lg:text-[13px] text-neutral-700 leading-relaxed font-medium list-disc pl-4 space-y-3 max-w-md"
          >
            <li>
              Graduated as a Full Graduate from a highly competitive Machine Learning academy
              endorsed by the Kampus Merdeka (MSIB) program.
            </li>
            <li>
              Mastered fundamental to advanced AI techniques, including Deep Learning, Generative
              Adversarial Networks (GANs), and Natural Language Processing (NLP) using TensorFlow
              and Python.
            </li>
            <li>
              Gained hands-on experience in extracting data insights, deploying Machine Learning
              models on the web, and structuring end-to-end ML workflows.
            </li>
            <li>
              Successfully collaborated on a final Capstone Project to develop an application that
              solves real-world problems and validates product development skills.
            </li>
          </ul>
        </div>

        <div class="mt-8 lg:mt-10 flex flex-col gap-2.5 md:pl-[50px] lg:pl-[100px]">
          <div class="flex items-start">
            <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">Led By</div>
            <div class="text-[11px] text-neutral-700 font-medium leading-tight">
              Google, GoTo, and Traveloka
            </div>
          </div>
          <div class="flex items-start">
            <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">Program</div>
            <div class="text-[11px] text-neutral-700 font-medium leading-tight">
              Kampus Merdeka (MSIB)
            </div>
          </div>
          <div class="flex items-start">
            <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">Period</div>
            <div class="text-[11px] text-neutral-700 font-medium leading-tight">
              09/2024 - 01/2025
            </div>
          </div>
          <div class="flex items-start">
            <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">Location</div>
            <div class="text-[11px] text-neutral-700 font-medium leading-tight">Pekanbaru</div>
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
