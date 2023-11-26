<script setup>
definePageMeta({
  middleware: defineNuxtRouteMiddleware(() => {
    console.log('[匿名中間件] 我是直接定義在頁面內的匿名中間件')
  })
})
</script>

<template>
  <div class="bg-white py-24">
    <div class="flex flex-col items-center">
      <h1 class="text-6xl font-semibold text-gray-800">
        這裡是首頁
      </h1>
      <div class="my-4 flex space-x-4">
        <NuxtLink to="/modules">前往modules</NuxtLink>
        <NuxtLink to="/composables">前往composables</NuxtLink>
        <NuxtLink to="/plugins">前往plugins</NuxtLink>
        <NuxtLink to="/middleware">前往middleware</NuxtLink>
      </div>
    </div>
  </div>
</template>
