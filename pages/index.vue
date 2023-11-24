<script setup lang="ts">
const { x, y } = useMouse()

const colorMode = useColorMode()

function toggleMode() {
  colorMode.value = colorMode.value === 'light' ? 'dark' : 'light'
}
</script>

<template>
  <div text-xl text-rose w-full px4 py2 flex="~ items-center justify-between">
    <div>
      {{ x }}, {{ y }}
    </div>
    <div>
      {{ colorMode.value }}
    </div>
    <button @click="toggleMode">
      <div i-carbon-sun dark:i-carbon-moon />
    </button>
  </div>
</template>
