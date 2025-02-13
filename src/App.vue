<script setup lang="ts">
import { ref } from 'vue'
import Contacts from './pages/Contacts.vue'
import Sidebar from './components/Sidebar.vue'
import Header from './components/Header.vue'

const showSidebar = ref(true)

const toggleSidebar = () => {
  showSidebar.value = !showSidebar.value
}
</script>

<template>
  <div class="bg-stone-700 h-screen">
    <div class="flex flex-col p-4" style="height: 100vh">
      <Header @toggle-sidebar="toggleSidebar" />

      <div class="flex w-full h-full">
        <div class="fixed left-0 z-20 sm:flex sm:relative">
          <Sidebar v-if="showSidebar" />
        </div>
        <div class="w-full h-full relative z-0">
          <Contacts />
        </div>
      </div>
    </div>
  </div>
</template>
