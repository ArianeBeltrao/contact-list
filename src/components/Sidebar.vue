<script setup lang="ts">
  import { Button } from '../components/ui/button'
</script>

<template>
    <div class="w-56 bg-yellow-100 h-full flex-none justify-between flex flex-col">
      <div>
        <div class="flex md:hidden p-8">
          Lista de contatos
        </div>

        <div class="flex flex-col m-3">
          <a class="px-4 py-2 flex w-full hover:bg-red-200 active:bg-blue-200 rounded-[48px]" href="#">
            <span>Contatos</span> 
          </a>
          <a class="px-4 py-2 flex w-full hover:bg-red-200 active:bg-blue-200 rounded-[48px]" href="#">
          <span>Meu Cadastro</span> 
          </a>
          <a class="px-4 py-2 flex w-full hover:bg-red-200 active:bg-blue-200 rounded-[48px]" href="#">
          <span>Usuários</span> 
          </a>
          <a class="px-4 py-2 flex w-full hover:bg-red-200 active:bg-blue-200 rounded-[48px]" href="#">
          <span>Pessoas</span> 
          </a>
        </div>

      </div>
     
      <div class="flex p-6">
        <Button class="w-full cursor-pointer hover:bg-red-200">Log out</Button>
      </div>
      
    </div>
  </template>
  

