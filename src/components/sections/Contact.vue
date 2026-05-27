<template>
  <section
    class="relative w-full h-[100svh] bg-[#ebebeb] overflow-hidden select-none flex flex-col justify-between text-[#1a1a1a] font-sans"
  >
    <BlueprintRuler position="top" :marker-index="20" />
    <BlueprintRuler position="bottom" :marker-index="75" />

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-10">
      <BlueprintGrid :rows="3" :cols="5" />
    </div>

    <div
      class="absolute top-12 left-6 md:top-12 md:left-12 text-[10px] md:text-[11px] font-bold tracking-widest text-neutral-900 z-30"
    >
      Fadhlur Rohman
    </div>
    <div
      class="absolute top-12 right-6 md:top-12 md:right-12 text-[10px] md:text-[11px] font-bold tracking-widest text-neutral-900 z-30"
    >
      @2026
    </div>

    <div class="absolute inset-0 flex items-center justify-center z-0 pointer-events-none">
      <h1
        class="text-[25vw] md:text-[16vw] font-serif text-neutral-400/50 blur-[3px] md:blur-[5px] tracking-tighter mix-blend-multiply opacity-60"
      >
        Portfolio
      </h1>
    </div>

    <div class="absolute inset-0 m-4 md:m-8 pointer-events-none z-30 flex flex-col justify-end">
      <div
        class="w-full grid grid-cols-2 md:grid-cols-5 gap-y-8 md:gap-y-0 items-end pb-4 md:pb-2 lg:pb-3 px-2 md:px-0"
      >
        <div class="col-span-1 pointer-events-auto pr-2 md:pr-4">
          <h4 class="text-[10px] font-bold uppercase tracking-widest text-neutral-900 mb-1.5">
            Email
          </h4>
          <a
            href="mailto:fadhlurrohman1204@gmail.com"
            class="text-[11px] lg:text-[12px] font-medium text-neutral-600 hover:text-neutral-900 hover:underline underline-offset-4 transition-all break-all md:break-normal block pr-2"
          >
            fadhlurrohman1204@gmail.com
          </a>
        </div>

        <div class="col-span-1 pointer-events-auto pr-2 md:pr-4">
          <h4 class="text-[10px] font-bold uppercase tracking-widest text-neutral-900 mb-1.5">
            Instagram
          </h4>
          <a
            href="https://www.instagram.com/lurrr.1/"
            target="_blank"
            class="text-[11px] lg:text-[12px] font-medium text-neutral-600 hover:text-neutral-900 hover:underline underline-offset-4 transition-all"
          >
            @Lurrr.1
          </a>
        </div>

        <div class="col-span-1 pointer-events-auto pr-2 md:pr-4">
          <h4 class="text-[10px] font-bold uppercase tracking-widest text-neutral-900 mb-1.5">
            LinkedIn
          </h4>
          <a
            href="https://linkedin.com/in/fadhlur-rohman-d1012"
            target="_blank"
            class="text-[11px] lg:text-[12px] font-medium text-neutral-600 hover:text-neutral-900 hover:underline underline-offset-4 transition-all"
          >
            Fadhlur Rohman
          </a>
        </div>

        <div class="col-span-1 pointer-events-auto pr-2 md:pr-4">
          <h4 class="text-[10px] font-bold uppercase tracking-widest text-neutral-900 mb-1.5">
            GitHub
          </h4>
          <a
            href="https://github.com/Lurrr1"
            target="_blank"
            class="text-[11px] lg:text-[12px] font-medium text-neutral-600 hover:text-neutral-900 hover:underline underline-offset-4 transition-all"
          >
            github.com/Lurrr1
          </a>
        </div>

        <div
          class="col-span-2 md:col-span-1 pointer-events-auto flex justify-start md:justify-end mt-4 md:mt-0"
        >
          <h2
            class="text-[3.5rem] md:text-6xl lg:text-[5.5rem] font-serif leading-[0.8] tracking-tight text-neutral-900 whitespace-nowrap md:translate-y-1 lg:translate-y-2"
          >
            Contact Me!
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
</style>
