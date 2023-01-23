<script setup lang="ts">
const links = {
  block1: [
    { name: 'About', url: '#' },
    { name: 'Advertising', url: '#' },
    { name: 'Business', url: '#' },
    { name: 'How Search works', url: '#' },
  ],
  block2: [
    { name: 'Privacy', url: '#' },
    { name: 'Terms', url: '#' },
  ],
};
</script>

<template>
  <footer
    class="flex justify-around bg-neutral-100 text-sm text-neutral-600 border-t leading-10"
  >
    <div class="flex gap-6">
      <a v-for="link in links.block1" :href="link.url">{{ link.name }}</a>
    </div>
    <div class="flex gap-6">
      <a v-for="link in links.block2" :href="link.url">{{ link.name }}</a>
    </div>
  </footer>
</template>
