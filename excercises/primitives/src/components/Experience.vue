<script setup lang="ts">
import { useRenderLoop } from '@tresjs/core';
import { Mesh, BoxGeometry, MeshBasicMaterial } from 'three'
import { ref } from 'vue';

const cube = new Mesh(
  new BoxGeometry(1, 1, 1),
  new MeshBasicMaterial({ color: 0xff0000 })
)

cube.position.set(0, 2, 0)

const { onLoop } = useRenderLoop()

const cubeRef = ref<Mesh>()
onLoop(() => {
  if (cubeRef.value) {
    cubeRef.value.rotation.y += 0.01
  }
})
</script>

<template>
  <TresPerspectiveCamera :position="[0, 5, 5]" :look-at="[0,0,0]" />
  <primitive :object="cube" :position="[2,2,0]" ref="cubeRef" />
  <TresGridHelper />
  <TresAxesHelper />
</template>
