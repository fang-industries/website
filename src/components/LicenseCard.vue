<template>
  <figure
    class="flex flex-col gap-y-2 rounded-2xl border-2 border-neutral-800 p-6"
  >
    <div class="text-xl font-medium text-lime-500 dark:text-lime-400">
      {{ props.name }}
    </div>
    <div class="font-medium">
      Licensed under the {{ props.license }} license.
    </div>
    <div class="text-neutral-700 dark:text-neutral-500">
      Copyright © {{ props.copyright }}
    </div>
  </figure>
</template>

<script setup lang="ts">
const props = defineProps<{
  name: string;
  license: string;
  copyright: string;
}>();
</script>
