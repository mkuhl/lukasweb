<script setup lang="ts">
import heroImage from '@/assets/main-img-nc.png'
import cursorGreen from '@/assets/cursor-green.png'
import cursorRed from '@/assets/cursor-red.png'

const portfolioPdfUrl = '/PORTFOLIO_LUKAS_KUHL.pdf'
const cvPdfUrl = '/CV_LUKAS_KUHL.pdf'
</script>

<template>
  <div class="min-h-screen bg-[#07032e] flex justify-center">
    <div class="relative w-[min(100vw,calc(100vh*240/294))] h-[min(100vh,calc(100vw*294/240))]">
      <img
        :src="heroImage"
        alt=""
        class="h-full w-full [image-rendering:pixelated]"
      />

      <!-- Green: title + cursor (CV download) -->
      <a
        :href="cvPdfUrl"
        class="absolute top-[7%] right-[13%] flex items-center gap-2 whitespace-nowrap"
        download
      >
        <h1 class="hero-title">lukas kuhl</h1>
        <img :src="cursorGreen" alt="" class="h-[min(3vh,3.5vw)] [image-rendering:pixelated]" />
      </a>

      <!-- Red: cursor + portfolio link -->
      <a
        :href="portfolioPdfUrl"
        class="absolute top-[67%] left-[51%] flex items-center gap-2 whitespace-nowrap"
        download
      >
        <img :src="cursorRed" alt="" class="h-[min(3vh,3.5vw)] [image-rendering:pixelated]" />
        <span class="btn-portfolio">portfolio</span>
      </a>
    </div>
  </div>
</template>
