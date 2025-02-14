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
  <div class="bg-stone-700 h-screen overflow-hidden">
    <div class="flex flex-col p-4" style="height: 100vh">
      <Header @toggle-sidebar="toggleSidebar" />

      <div class="flex w-full h-full">
        <Sidebar v-if="showSidebar" />

        <Contacts />
      </div>
    </div>
  </div>
</template>
