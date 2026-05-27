<template>
  <div
    :class="[
      'absolute left-0 w-full h-8 md:h-12 flex pointer-events-none z-20 px-2 overflow-hidden',
      position === 'top' ? 'top-0 items-start' : 'bottom-0 items-end',
    ]"
  >
    <div
      :class="[
        'relative w-full flex justify-between opacity-30',
        position === 'top' ? 'items-start' : 'items-end',
      ]"
    >
      <div v-for="i in 120" :key="i" class="relative flex justify-center">
        <div
          :class="[
            'w-[1px] bg-neutral-800',
            i % 10 === 0 ? 'h-4 md:h-6' : i % 5 === 0 ? 'h-3 md:h-4' : 'h-1.5 md:h-2',
          ]"
        ></div>

        <div
          v-if="i === markerIndex"
          class="absolute flex flex-col items-center z-30 opacity-100"
          :class="position === 'top' ? 'top-0' : 'bottom-0'"
        >
          <svg
            v-if="position === 'bottom'"
            class="w-[8px] md:w-[10px] h-[5px] md:h-[6px] fill-neutral-900 mb-[-1px]"
            viewBox="0 0 10 6"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path d="M0 0 L10 0 L5 6 Z" />
          </svg>

          <div class="w-[1.5px] md:w-[2px] h-5 md:h-8 bg-neutral-900"></div>

          <svg
            v-if="position === 'top'"
            class="w-[8px] md:w-[10px] h-[5px] md:h-[6px] fill-neutral-900 mt-[-1px]"
            viewBox="0 0 10 6"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path d="M5 0 L10 6 L0 6 Z" />
          </svg>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  position: {
    type: String,
    default: 'bottom', // 'top' atau 'bottom'
  },
  markerIndex: {
    type: Number,
    default: null, // Contoh: 10
  },
})
</script>
