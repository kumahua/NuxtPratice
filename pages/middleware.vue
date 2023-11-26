<template>
  <div class="bg-white py-24">
    <div class="flex flex-col items-center">
      <h1 class="text-6xl font-bold text-green-400">
        大家好！ 我是Darren
      </h1>
      <p class="my-8 text-3xl text-gray-600">
        這裡是/middleware
      </p>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  // 可以透過陣列來表示使用多個中間件
  middleware: ['random-redirect', 'named-test']
})
</script>