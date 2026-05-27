<template>
  <div class="relative w-full h-full">
    <template v-if="showLines">
      <template v-for="(vLinePos, index) in colPositions" :key="'v-' + index">
        <div
          v-if="!outlineOnly || index === 0 || index === colPositions.length - 1"
          class="absolute -top-[100vh] -bottom-[100vh] w-[1px] bg-neutral-400/50 pointer-events-none"
          :class="{
            /* Menyembunyikan garis selain kiri, tengah, kanan di layar HP */
            'hidden md:block': hideInnerOnMobile && !isMobileVisible(index, cols),
          }"
          :style="{ left: vLinePos }"
        ></div>
      </template>

      <template v-for="(hLinePos, index) in rowPositions" :key="'h-' + index">
        <div
          v-if="!outlineOnly || index === 0 || index === rowPositions.length - 1"
          class="absolute left-0 right-0 h-[1px] bg-neutral-400/50 pointer-events-none"
          :class="{
            /* Menyembunyikan garis selain atas, tengah, bawah di layar HP */
            'hidden md:block': hideInnerOnMobile && !isMobileVisible(index, rows),
          }"
          :style="{ top: hLinePos }"
        ></div>
      </template>
    </template>

    <template v-if="showMarkers">
      <template v-for="(yPos, rIndex) in rowPositions" :key="'row-' + rIndex">
        <template v-for="(xPos, cIndex) in colPositions" :key="'plus-' + cIndex + '-' + rIndex">
          <span
            v-if="
              !outlineOnly ||
              rIndex === 0 ||
              rIndex === rowPositions.length - 1 ||
              cIndex === 0 ||
              cIndex === colPositions.length - 1
            "
            class="absolute text-sm font-light leading-none bg-transparent z-10 pointer-events-none"
            :class="[
              getMarkerColor(rIndex * cols + cIndex),
              {
                /* Sembunyikan tanda '+' jika BUKAN bagian dari formasi 3x3 di HP
                 */
                'hidden md:block':
                  hideInnerOnMobile &&
                  (!isMobileVisible(rIndex, rows) || !isMobileVisible(cIndex, cols)),

                /* Dukungan opsional jika Anda menggunakan prop hide-center-plus */
                hidden: hideCenterPlus && isCenter(rIndex, rows) && isCenter(cIndex, cols),
              },
            ]"
            :style="{ top: yPos, left: xPos, transform: 'translate(-50%, -50%)' }"
            >+</span
          >
        </template>
      </template>
    </template>

    <slot></slot>
  </div>
</template>

<script setup>
import { computed } from 'vue'

const props = defineProps({
  rows: { type: Number, default: 3 },
  cols: { type: Number, default: 5 },
  outlineOnly: { type: Boolean, default: false },
  hideInnerOnMobile: { type: Boolean, default: true },
  hideCenterPlus: { type: Boolean, default: false }, // Mengamankan jika dipakai di section tertentu
  whiteMarkers: { type: Array, default: () => [] },
  blackMarkers: { type: Array, default: () => [] },
  showLines: { type: Boolean, default: true },
  showMarkers: { type: Boolean, default: true },
})

const calculatePositions = (count) => {
  if (count <= 1) return ['50%']
  const positions = []
  for (let i = 0; i < count; i++) {
    positions.push(`${(i / (count - 1)) * 100}%`)
  }
  return positions
}

const rowPositions = computed(() => calculatePositions(props.rows))
const colPositions = computed(() => calculatePositions(props.cols))

const getMarkerColor = (index) => {
  if (props.whiteMarkers.includes(index)) return 'text-white'
  if (props.blackMarkers.includes(index)) return 'text-neutral-900'
  return 'text-neutral-500'
}

/* LOGIKA MAGIC (3x3 HP):
  Fungsi ini akan memeriksa posisi index.
  Hanya index [Awal], [Tengah], dan [Akhir] yang diizinkan tampil di mobile.
*/
const isMobileVisible = (index, totalCount) => {
  if (index === 0) return true // Tampilkan paling kiri/atas
  if (index === totalCount - 1) return true // Tampilkan paling kanan/bawah
  if (index === Math.floor((totalCount - 1) / 2)) return true // Tampilkan titik tengah persis
  return false // Sembunyikan sisanya
}

// Cek titik tengah absolut untuk properti hideCenterPlus
const isCenter = (index, totalCount) => index === Math.floor((totalCount - 1) / 2)
</script>
