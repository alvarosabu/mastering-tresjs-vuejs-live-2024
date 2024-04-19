<script setup lang="ts">
import Sphere from './Sphere.vue'
import Cylinder from './Cylinder.vue'
import Torus from './Torus.vue'
import TorusKnot from './TorusKnot.vue'
</script>

<template>
  <TresPerspectiveCamera :position="[5, 5, 5]" :look-at="[0,0,0]" />
  <TresMesh>
    <TresBoxGeometry :args="[1,1,1]" :position="[0,1,0]" />
    <TresMeshNormalMaterial  />
  </TresMesh>
  <Sphere />
  <Cylinder :args="[0.5, 0.5, 1, 32]" :position="[-2, 0, 0]" />
  <Torus />
  <TorusKnot />
  <TresGridHelper />
  <TresAxesHelper />
</template>
