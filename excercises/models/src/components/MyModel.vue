<script setup lang="ts">
import { useGLTF } from '@tresjs/cientos';

const { nodes, materials } = await useGLTF('https://raw.githubusercontent.com/Tresjs/assets/main/models/gltf/aku-aku/AkuAku.gltf')

console.log({nodes, materials})
</script>

<template>
  <primitive :object="nodes.AkuAku" />
</template>