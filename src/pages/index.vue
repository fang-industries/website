<template>
  <main class="flex min-h-screen flex-col justify-between py-8">
    <Navbar />
    <div class="min-w-screen flex justify-center">
      <div class="flex flex-col gap-y-8 text-center">
        <img src="@/assets/branding/fard.svg" class="h-24" />
        <blockquote class="text-xl">We do shit.</blockquote>
      </div>
    </div>
    <Footer />
  </main>
</template>

<script setup lang="ts">
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
</script>
