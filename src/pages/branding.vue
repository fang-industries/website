<template>
  <main class="flex flex-col gap-y-16 py-8">
    <Navbar />
    <div class="min-w-screen flex justify-center px-8 md:px-0">
      <div class="flex w-[48rem] flex-col gap-y-16 text-center">
        <div class="flex flex-col gap-y-8">
          <div class="flex flex-col gap-y-4">
            <h1 class="text-5xl font-semibold">Design & Branding</h1>
            <p>
              The Fang Industries, inc. brand belongs to Pix3l_, the entity that
              guides and supports Fang Industries, inc. These guidelines
              describe when and how the brand should be used.
            </p>
          </div>
          <div class="flex flex-col gap-y-4">
            <h2 class="text-4xl font-medium">Brand Marks</h2>
            <p>
              Fang Industries, inc. claims ownership over one mark: The
              <strong>Fang Industries, inc. logo-type</strong>.
            </p>
          </div>
          <div class="flex flex-col gap-y-4">
            <h2 class="text-xl font-medium">
              Both said marks should be used with the following in mind:
            </h2>
            <ul>
              <li>
                Do not stretch, skew, rotate, flip, or otherwise alter the
                marks.
              </li>
              <li>
                Do not use the marks on an overly-busy background; solid colours
                or gradients work best.
              </li>
            </ul>
          </div>
        </div>
        <div class="flex flex-col gap-y-8">
          <div class="flex flex-col gap-y-4">
            <img
              src="@/assets/branding/fard.svg"
              class="h-24"
              alt="Fang Industries, inc. - Main Logo-type"
            />
            <figcaption
              class="font-semibold text-neutral-600 dark:text-neutral-500"
            >
              Fang Industries, inc. - Main Logo-type
            </figcaption>
          </div>
          <div class="flex flex-col gap-y-4 md:flex-row md:gap-8">
            <div class="flex flex-col gap-y-4">
              <img
                src="@/assets/branding/fard-light.svg"
                class="h-24"
                alt="Fang Industries, inc. - Main Logo-type"
              />
              <figcaption
                class="font-semibold text-neutral-600 dark:text-neutral-500 md:text-sm"
              >
                Fang Industries, inc. - White Logo-type
              </figcaption>
            </div>
            <div class="flex flex-col gap-y-4">
              <img
                src="@/assets/branding/fard-dark.svg"
                class="h-24"
                alt="Fang Industries, inc. - Main Logo-type"
              />
              <figcaption
                class="font-semibold text-neutral-600 dark:text-neutral-500 md:text-sm"
              >
                Fang Industries, inc. - Black Logo-type
              </figcaption>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </main>
</template>

<script setup lang="ts">
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
</script>
