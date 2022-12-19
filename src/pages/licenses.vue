<template>
  <main class="space-y-16 py-8">
    <Navbar />
    <section id="heading">
      <div class="flex w-[48rem] flex-col gap-y-4 px-8 md:px-0">
        <h1 class="text-4xl font-semibold">License Notice</h1>
        <p class="text-neutral-500 dark:text-neutral-400">
          This project uses external assets and open-source libraries, and would
          like to give attribution.
        </p>
      </div>
    </section>
    <section id="members">
      <div class="grid w-[48rem] grid-cols-2 flex-col gap-6 px-8 md:px-0">
        <LicenseCard
          name="Vue"
          license="MIT"
          copyright="2013-present, Yuxi (Evan) You"
        />
        <LicenseCard
          name="Vue Router"
          license="MIT"
          copyright="2013-present, Yuxi (Evan) You"
        />
        <LicenseCard
          name="Tailwind CSS"
          license="MIT"
          copyright="Tailwind Labs, Inc."
        />
        <LicenseCard
          name="Autoprefixer"
          license="MIT"
          copyright="2013 Andrey Sitnik"
        />
        <LicenseCard
          name="PostCSS"
          license="MIT"
          copyright="2013 Andrey Sitnik"
        />
        <LicenseCard
          name="Unplugin Icons"
          license="MIT"
          copyright="2020 Anthony Fu"
        />
      </div>
    </section>
    <Footer />
  </main>
</template>

<script setup lang="ts">
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import LicenseCard from "@/components/LicenseCard.vue";
</script>
