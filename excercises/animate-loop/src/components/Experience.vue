<script setup lang="ts">
import { useRenderLoop } from '@tresjs/core';
import { ref } from 'vue';

const boxRef = ref()
const { onLoop } = useRenderLoop()

onLoop(({ delta, elapsed }) => {
  if(boxRef.value) {
    boxRef.value.rotation.y += delta
    boxRef.value.rotation.z = elapsed
  }
})
</script>

<template>
  <TresPerspectiveCamera :position="[5, 5, 5]" :look-at="[0,0,0]" />
  <TresMesh ref="boxRef" :position="[0,2,0]" :rotation="[-Math.PI/3, 0 , 0]">
    <TresBoxGeometry :args="[1,1,1]"  />
    <TresMeshNormalMaterial  />
  </TresMesh>
  <TresGridHelper />
  <TresAxesHelper />
</template>
