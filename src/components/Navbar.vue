<template>
  <div class="flex w-full justify-center">
    <div class="w-[48rem]">
      <div class="flex w-full justify-between px-8 md:px-0">
        <router-link
          to="/"
          :class="
            $route.path === '/'
              ? `cursor-default font-semibold text-lime-600 dark:text-lime-400`
              : `underline transition hover:text-lime-700 dark:hover:text-lime-200`
          "
          >Home</router-link
        >

        <div class="flex">
          <router-link
            to="/employees"
            :class="
              $route.path === '/employees'
                ? `cursor-default font-semibold text-lime-600 dark:text-lime-400`
                : `underline transition hover:text-lime-700 dark:hover:text-lime-200`
            "
            >Employees</router-link
          >
        </div>
      </div>
    </div>
  </div>
</template>
