<script setup lang="ts">
import Contacts from './pages/Contacts.vue';
import Sidebar from './components/Sidebar.vue';
</script>

<template>
  <div class="bg-dark h-screen">
    <div class="flex flex-col" style="height: 100vh;">
      <div class="sticky top-0 p-2 flex items-center justify-between w-full bg-blue-300">
        HEADER
      </div>
      <div class="flex w-full h-full">
        <Sidebar/>
        <div class="w-full h-full relative">
          <Contacts />
        </div>
      </div>
    </div>
  </div>

</template>
