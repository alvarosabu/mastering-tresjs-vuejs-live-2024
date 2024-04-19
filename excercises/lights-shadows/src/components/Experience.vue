<script setup lang="ts">
import { vLightHelper } from '@tresjs/core';
</script>

<template>
  <TresPerspectiveCamera :position="[9,9,9]" :look-at="[0,0,0]" />
  <TresMesh cast-shadow :position="[0,2,0]">
    <TresSphereGeometry :args="[1,32,32]"  />
    <TresMeshToonMaterial color="teal"  />
  </TresMesh>
  <TresMesh receive-shadow>
    <TresPlaneGeometry :args="[20, 20, 100, 100]" :rotate-x="-Math.PI/2" />
    <TresMeshToonMaterial color="lightgray"  />
  </TresMesh>
  <TresAxesHelper />
  <TresAmbientLight :intensity="0.5" />
  <TresPointLight
    :position="[2, 0, 1]"
    :args="['#ff7d46', 1, 7]"
  />
  <TresDirectionalLight
    v-light-helper
    :position="[5,6,-2]"
    :intensity="2"
    color="cyan"
    cast-shadow
    :shadow-mapSize-width="1024"
    :shadow-mapSize-height="1024"
    :shadow-camera-near="0.1"
    :shadow-camera-far="100"
  />
  <TresSpotLight
    v-light-helper
    :position="[-5, 5, 5]"
    :intensity="12"
    :args="['#ffffff', 3.6, 10, Math.PI * 0.3]"
  />
</template>
