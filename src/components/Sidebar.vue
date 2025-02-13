<script setup lang="ts">
import { Button } from '../components/ui/button'

const menuItems = [
  { name: 'Contatos', path: '/contacts' },
  { name: 'Meu Cadastro', path: '/meu-cadastro' },
  { name: 'Usuários', path: '/usuarios' },
  { name: 'Pessoas', path: '/pessoas' },
]
</script>

<template>
  <div
    class="sm:w-72 w-40 h-full flex-none justify-between flex flex-col bg-stone-700"
  >
    <div class="flex flex-col m-3">
      <router-link
        v-for="item in menuItems"
        :key="item.path"
        :to="item.path"
        class="px-4 py-2 text-white flex w-full hover:bg-sky-200 hover:text-stone-700 active:bg-blue-200 rounded-[48px] cursor-pointer"
      >
        <span>{{ item.name }}</span>
      </router-link>
    </div>

    <div class="flex">
      <Button
        class="w-full cursor-pointer bg-sky-200 text-stone-700 hover:bg-sky-300"
      >
        Log out</Button
      >
    </div>
  </div>
</template>
