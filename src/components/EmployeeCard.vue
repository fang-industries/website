<template>
  <figure
    class="flex flex-col gap-x-8 gap-y-8 rounded-2xl border-2 border-neutral-800 p-6 md:flex-row"
  >
    <img
      :src="props.img"
      class="my-auto mx-auto h-24 w-24 rounded-full object-cover md:mx-0"
      :alt="`A picture of ${props.name}.`"
    />
    <div class="flex flex-col justify-between gap-y-4">
      <blockquote>
        <p class="text-lg font-medium">“{{ props.quote }}”</p>
      </blockquote>
      <figcaption>
        <div class="font-medium text-lime-500 dark:text-lime-400">
          {{ props.name }}
        </div>
        <div class="text-neutral-700 dark:text-neutral-500">
          Joined {{ calculateTimestamp(props.timestamp) }}
        </div>
      </figcaption>
    </div>
  </figure>
</template>

<script setup lang="ts">
const props = defineProps<{
  img: string;
  quote: string;
  name: string;
  timestamp: number;
}>();

const date = new Date();
const timestamp = date.getTime();
const seconds = Math.floor(timestamp / 1000);

function calculateTimestamp(memberJoin: number) {
  const oldTimestamp = memberJoin;
  const diff = seconds - oldTimestamp;

  if (diff < 60) {
    return `${diff} seconds ago`;
  } else if (diff < 3600) {
    return `${Math.floor(diff / 60)} minutes ago`;
  } else if (diff < 86400) {
    return `${Math.floor(diff / 3600)} hours ago`;
  } else if (diff < 2620800) {
    return `${Math.floor(diff / 86400)} days ago`;
  } else if (diff < 31449600) {
    return `${Math.floor(diff / 2620800)} months ago`;
  } else {
    return `${Math.floor(diff / 31449600)} years ago`;
  }
}
</script>
