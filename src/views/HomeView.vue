<script setup lang="ts">
import heroImage from '@/assets/main-img.png'

const portfolioPdfUrl = '/portfolio.pdf'
</script>

<template>
  <div class="min-h-screen bg-[#07032e] flex justify-center">
    <div class="relative w-[min(100vw,calc(100vh*240/294))] h-[min(100vh,calc(100vw*294/240))]">
      <img
        :src="heroImage"
        alt=""
        class="h-full w-full [image-rendering:pixelated]"
      />
      <h1 class="hero-title absolute top-[7.7%] right-[26%]">lukas kuhl</h1>
      <a
        :href="portfolioPdfUrl"
        class="btn-portfolio absolute top-[67.5%] left-[58%]"
        download
      >
        PORTFOLIO
      </a>
    </div>
  </div>
</template>
