<script setup lang="ts">
</script>

<template>
  <TresPerspectiveCamera :position="[3, 3, 3]" :look-at="[0,0,0]" />
  <TresAxesHelper />
  <TresGridHelper />
  <TresAmbientLight :intensity="1" />
</template>
