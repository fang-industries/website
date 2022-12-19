<template>
  <div class="flex w-full justify-center">
    <div class="w-[48rem]">
      <div class="flex w-full justify-between px-8 md:px-0">
        <div class="text-neutral-500 dark:text-neutral-400">
          Copyright © 2022 Fang Industries, inc.
        </div>
        <div class="flex">
          <router-link
            to="/licenses"
            :class="
              $route.path === '/licenses'
                ? `cursor-default font-semibold text-lime-600 dark:text-lime-400`
                : `underline transition hover:text-lime-700 dark:hover:text-lime-200`
            "
            >Licenses</router-link
          >
        </div>
      </div>
    </div>
  </div>
</template>
