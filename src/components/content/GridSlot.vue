<script setup lang="ts">
defineProps({
  title: {
    type: String,
    default: 'Uses Slot title',
  },
})
</script>

<template>
  <li class="group relative flex flex-col items-start">
    <h3 class="text-base font-semibold tracking-tight text-zinc-800 dark:text-zinc-100">
      {{ title }}
    </h3>
    <p class="relative z-10 mt-2 text-sm text-zinc-600 dark:text-zinc-400">
      <slot />
    </p>
  </li>
</template>
