<script setup>
const loading = ref(false)
</script>

<template>
  <div class="grid w-full gap-4">
    <header class="flex items-start justify-between">
      <div class="grow">
        <p>Hi, welcome back Gumzhbond</p>
        <h1>Dashboard</h1>
      </div>
      <div class="w-[120px] h-[36px] bg-neutral-200"></div>
    </header>
    <main class="grid gap-4">
      <div class="flex items-center gap-3">
        <!-- Tabs: Today This week This month This year -->
        <div v-for="(item, index) in 3" :key="index" class="w-[120px] h-[36px] bg-neutral-200"></div>
      </div>
      <section>
        <!-- Chart -->
        <div class="w-full h-[360px] bg-neutral-200"></div>
      </section>
    </main>
    <footer>
      <!-- I'll have 3 differents cards -->
       <div class="flex items-center gap-4">
        <div v-for="(item, index) in 3" :key="index" class="w-full h-[260px] bg-neutral-200"></div>
       </div>
    </footer>
  </div>
</template>

<style></style>