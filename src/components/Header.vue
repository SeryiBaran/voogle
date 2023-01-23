<script setup lang="ts">
import { Icon } from '@iconify/vue';
import Button from '@/components/Button.vue';
</script>

<template>
  <header class="flex justify-end items-center gap-6 py-3 px-4">
    <div class="flex text-sm gap-4">
      <a href="">Gmail</a>
      <a href="">Images</a>
    </div>
    <button><Icon icon="mdi:dots-grid" width="24" height="24" /></button>
    <Button primary isLink href="https://accounts.google.com">Sign in</Button>
  </header>
</template>
