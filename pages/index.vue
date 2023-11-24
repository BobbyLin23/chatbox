<script setup lang="ts">
const { x, y } = useMouse()
</script>

<template>
  <div text-2xl text-rose>
    Hello World
    <div>
      {{ x }}, {{ y }}
    </div>
  </div>
</template>
