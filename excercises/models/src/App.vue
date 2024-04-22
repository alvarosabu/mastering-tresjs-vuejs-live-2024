<script setup lang="ts">
import { TresCanvas } from '@tresjs/core'
import Experience from './components/Experience.vue'
</script>

<template>
  <TresCanvas window-size clear-color="#82DBC5" alpha>
    <Experience />
  </TresCanvas>
</template>
