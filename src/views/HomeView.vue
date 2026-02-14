<script setup lang="ts">
const portfolioPdfUrl = '/portfolio.pdf'
</script>

<template>
  <div class="min-h-screen bg-secondary flex items-center justify-center">
    <div class="container-site text-center">
      <h1 class="hero-title text-primary mb-8">Lukas Kuhl</h1>
      <p class="text-xl md:text-2xl text-primary/70 mb-12">Artist Portfolio</p>
      <a :href="portfolioPdfUrl" class="btn-primary inline-block" download>
        Download Portfolio
      </a>
    </div>
  </div>
</template>
