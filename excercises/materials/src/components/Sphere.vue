<template>
  <TresMesh :position="[2, 0, 0]">
    <TresSphereGeometry :args="[0.75, 32, 32]"   />
    <TresMeshStandardMaterial color="#049ef4" :roughness="0.2" />
  </TresMesh>
</template>