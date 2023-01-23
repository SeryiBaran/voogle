<script setup lang="ts">
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';
import SearchForm from '@/components/SearchForm.vue';
import Button from '@/components/Button.vue';
</script>

<template>
  <div class="flex flex-col h-screen">
    <Header />
    <main class="grow flex flex-col items-center py-24 gap-7">
      <img src="@/assets/googleLogo.png" alt="" />
      <SearchForm />
      <div class="flex gap-3">
        <Button>Google Search</Button>
        <Button>I'm Feeling Lucky</Button>
      </div>
    </main>
    <Footer />
  </div>
</template>
