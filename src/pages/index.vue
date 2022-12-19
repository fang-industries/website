<template>
  <main class="flex min-h-screen flex-col justify-between py-8">
    <Navbar />
    <div class="min-w-screen flex justify-center px-8 md:px-0"></div>
    <Footer />
  </main>
</template>

<script setup lang="ts">
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
</script>
