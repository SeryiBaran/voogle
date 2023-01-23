<script setup lang="ts">
defineProps<{
  primary?: boolean;
  isLink?: boolean;
}>();
</script>

<template>
  <component
    :is="isLink ? 'a' : 'button'"
    class="rounded px-6 py-1.5 text-sm hover:shadow-lg active:shadow-lg border border-transparent"
    :class="[
      primary
        ? 'text-white bg-blue-600 font-medium'
        : 'bg-neutral-100 hover:border-inherit active:border-inherit focus:border-blue-600',
    ]"
  >
    <slot />
  </component>
</template>
