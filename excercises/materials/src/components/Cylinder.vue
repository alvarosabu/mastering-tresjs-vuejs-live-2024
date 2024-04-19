<script setup lang="ts">
defineProps<{
  args: [number, number, number, number]
  position: [number, number, number]
}>()

</script>

<template>
  <TresMesh :position="position">
    <TresCylinderGeometry :args="args"   />
    <TresMeshStandardMaterial color="yellow" transparent :opacity="0.5"/>
  </TresMesh>
</template>