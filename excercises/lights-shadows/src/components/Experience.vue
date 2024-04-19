<script setup lang="ts">
</script>

<template>
  <TresPerspectiveCamera :position="[0, 5, 5]" :look-at="[0,0,0]" />
  <TresGridHelper />
  <TresAxesHelper />
</template>
