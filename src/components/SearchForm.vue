<script setup lang="ts">
import { ref } from 'vue';

import { Icon } from '@iconify/vue';

import GoogleMicrophone from '@/icons/GoogleMicrophone.vue';
import GoogleCamera from '@/icons/GoogleCamera.vue';

const isFocused = ref(false);
</script>

<template>
  <form
    action="https://google.com/search?q=q"
    autocomplete="no"
    class="border rounded-full max-w-xl w-full flex space-x-4 px-4 items-center hover:shadow-md"
    :class="{ 'shadow-md': isFocused }"
  >
    <Icon icon="mdi:magnify" color="#9aa0a6" width="22" height="22" />
    <input
      @focus="isFocused = true"
      @blur="isFocused = false"
      class="h-11 grow"
      type="text"
      name="q"
    />
    <GoogleCamera class="h-6 w-6" />
    <GoogleMicrophone class="h-6 w-6" />
  </form>
</template>

<style scoped></style>
