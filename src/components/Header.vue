<script setup lang="ts">
import 'primeicons/primeicons.css'
import { defineEmits } from 'vue'

const emit = defineEmits(['toggle-sidebar'])
</script>

<template>
  <header
    class="h-16 sticky top-0 flex items-center justify-between sm:justify-start w-full gap-6"
  >
    <button
      @click="emit('toggle-sidebar')"
      class="flex h-10 w-10 rounded-full items-center justify-center cursor-pointer hover:bg-gray-50"
    >
      <i class="pi pi-bars text-sky-200" style="font-size: 1.5rem"></i>
    </button>
    <div class="flex justify-center gap-4 items-center">
      <i class="pi pi-user text-sky-200" style="font-size: 2.5rem"></i>
      <h1 class="hidden sm:flex font-[Comfortaa] text-3xl text-sky-200">
        agenda
      </h1>
    </div>

    <!-- <div class="flex h-20 w-20 bg-cyan-500">primary blue</div>
    <div class="flex h-20 w-20 bg-cyan-600">primary blue</div>
    <div class="flex h-20 w-20 bg-cyan-700">primary blue</div>
    <div class="flex h-20 w-20 bg-sky-200">usando no header</div>
    <div class="flex h-20 w-20 bg-sky-400">primary blue</div> -->
  </header>
</template>
