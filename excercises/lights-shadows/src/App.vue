<script setup lang="ts">
import { TresCanvas } from '@tresjs/core'
import Experience from './components/Experience.vue'
</script>

<template>
  <TresCanvas window-size clear-color="#000000" shadows>
    <Experience />
  </TresCanvas>
</template>
