<script setup lang="ts">
import { isDark, toggleDark } from '~/composables'

</script>

<template>
  <div id="menu-container" w="full" class="fixed p-2 z-49 text-light-50">
  <nav id="menubar" w="full" class="text-lg z-50 mt-1">
    <router-link class="icon-btn mx-2" to="/">
      <codicon:home /><div style="top:-4px;" class="mx-4 relative inline-block"></div>
    </router-link>


    <router-link class="icon-btn mx-2" to="/slides/theory">
       <carbon:research-hinton-plot /><div style="top:-4px;" class="mx-4 relative inline-block">1. Предпосылки</div>
    </router-link>

    <router-link class="icon-btn mx-2" to="/slides/data" >
       <carbon:data-view-alt /><div style="top:-4px;" class="mx-4 relative inline-block">2. Данные</div>
    </router-link>

    <router-link class="icon-btn mx-2" to="/slides/excel" >
       <carbon:chart-line-data /><div style="top:-4px;" class="mx-4 relative inline-block">3. Первичный анализ</div>
    </router-link>

    <router-link class="icon-btn mx-2" to="/slides/model">
       <carbon:ai-status /><div style="top:-4px;" class="mx-4 relative inline-block">4. Модель</div>
    </router-link>

    <router-link class="icon-btn mx-2" to="/slides/exit">
       <bytesize:sign-in /><div style="top:-4px;" class="mx-4 relative inline-block">5. Вывод</div>
    </router-link>

    <button class="icon-btn mx-2 !outline-none" @click="toggleDark()">
      <carbon-moon v-if="isDark" />
      <carbon-sun v-else />
    </button>

  </nav>
  </div>
</template>

<style>
#menu-container {
  top: 0px;
  background-color: #161b22;
  left: 0px;
  opacity: 1 !important;
}

</style>
