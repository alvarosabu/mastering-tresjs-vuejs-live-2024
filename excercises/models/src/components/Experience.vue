<script setup lang="ts">
import MyModel from './MyModel.vue'
</script>

<template>
  <TresPerspectiveCamera :position="[9,9,9]" :look-at="[0,0,0]" />
  <TresDirectionalLight color="#F78B3D" :position="[3, 3, 3]" :intensity="1" />

  <Suspense>
    <MyModel />
  </Suspense>
  <TresAmbientLight :intensity="2" />>
</template>
