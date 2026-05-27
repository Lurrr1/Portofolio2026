<template>
  <section
    class="relative w-full h-auto md:h-screen bg-[#ebebeb] text-[#1a1a1a] font-sans md:overflow-hidden select-none py-16 md:py-0"
  >
    <BlueprintRuler position="top" :marker-index="20" class="z-50" />
    <BlueprintRuler position="bottom" :marker-index="50" class="z-50" />

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-20">
      <BlueprintGrid
        :rows="3"
        :cols="5"
        :white-markers="[3, 8, 13]"
        :black-markers="[0, 1, 2, 4, 5, 6, 7, 9, 10, 11, 12, 14]"
      />
    </div>

    <div
      class="relative md:absolute md:inset-0 m-4 md:m-8 p-6 md:p-0 flex flex-col md:flex-row gap-10 md:gap-0 pointer-events-auto"
    >
      <div
        class="w-full md:w-1/2 h-auto md:h-full flex flex-col justify-center p-0 md:px-8 lg:px-12 py-8 md:py-12 relative md:border-r border-neutral-300/30 z-30"
      >
        <div class="flex flex-col w-full my-auto">
          <div class="md:hidden text-[11px] font-bold tracking-widest text-neutral-900 mb-2">
            06
          </div>

          <div
            class="text-[10px] font-bold uppercase tracking-[0.2em] text-neutral-500 mb-3 md:mb-4"
          >
            Undergraduate Thesis
          </div>

          <h2
            class="text-[2.5rem] md:text-4xl lg:text-[3.5rem] font-serif leading-[1] md:leading-[1.05] tracking-tight text-neutral-900 mb-4 md:mb-6 mt-0"
          >
            Empathetic<br />AI Assistant.
          </h2>

          <ul
            class="text-[11px] lg:text-[13px] text-neutral-700 leading-relaxed font-medium list-disc pl-4 space-y-1.5 md:space-y-2 max-w-md pr-2 mb-6 md:mb-8"
          >
            <li>
              Developed an AIoT-based virtual assistant designed to provide light psychological
              support by recognizing real-time emotional states.
            </li>
            <li>
              Integrated an ESP32-S3 wearable to simultaneously capture voice inputs and
              physiological signals (heart rate, GSR, temperature, and acceleration).
            </li>
            <li>
              Engineered a multimodal fusion pipeline using OpenAI's Whisper for speech-to-text,
              IndoBERT for text emotion classification, and WESAD-trained models for physiological
              analysis.
            </li>
            <li>
              Leveraged Large Language Models (LLM) to generate highly contextual, empathetic
              responses delivered via a Text-to-Speech (TTS) audio system.
            </li>
            <li>
              Designed a responsive Vue.js web dashboard to continuously monitor user physiological
              trends, conversation history, and real-time emotion graphs.
            </li>
          </ul>

          <div class="flex flex-col gap-1.5 md:gap-2">
            <div class="flex items-start">
              <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">Domain</div>
              <div class="text-[11px] text-neutral-700 font-medium leading-tight">
                AIoT & NLP (Mental Health)
              </div>
            </div>
            <div class="flex items-start">
              <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">
                Tech Stack
              </div>
              <div class="text-[11px] text-neutral-700 font-medium leading-tight">
                ESP32-S3, Python, FastAPI, Vue.js
              </div>
            </div>
            <div class="flex items-start">
              <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">
                AI Models
              </div>
              <div class="text-[11px] text-neutral-700 font-medium leading-tight">
                Whisper, IndoBERT, LLM, TTS
              </div>
            </div>
            <div class="flex items-start">
              <div class="w-24 md:w-28 text-[11px] font-bold text-neutral-900 shrink-0">
                Location
              </div>
              <div class="text-[11px] text-neutral-700 font-medium leading-tight">
                Universitas Islam Riau (2026)
              </div>
            </div>
          </div>
        </div>
      </div>

      <div
        class="w-full md:w-1/2 h-auto md:h-full flex items-center justify-center md:justify-end relative mt-4 md:mt-0 mb-8 md:mb-0 z-10"
      >
        <div
          class="hidden md:block absolute top-4 right-6 text-[11px] font-bold tracking-widest text-black mix-blend-difference z-50 pointer-events-none"
        >
          06
        </div>

        <div
          class="w-full md:w-[calc(100%+2rem)] aspect-square md:aspect-auto md:h-[75%] lg:h-[80%] bg-neutral-300 overflow-hidden shadow-2xl ring-1 ring-neutral-400/50 grid grid-cols-2 grid-rows-2 gap-0"
        >
          <div
            class="col-span-2 row-span-1 bg-neutral-400 overflow-hidden group cursor-pointer relative border-b border-neutral-100/20"
          >
            <img
              src="../../../public/images/Sempro.webp"
              alt="Sempro"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>

          <div
            class="col-span-1 row-span-1 bg-neutral-400 overflow-hidden group cursor-pointer relative border-r border-neutral-100/20"
          >
            <img
              src="../../../public/images/Samantha.webp"
              alt="Samantha"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-1000"
            />
          </div>

          <div
            class="col-span-1 row-span-1 bg-neutral-400 overflow-hidden group cursor-pointer relative"
          >
            <img
              src="../../../public/images/Pose.webp"
              alt="Pose"
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
