<template>
  <TresMesh :position="[4, 0, 0]">
    <TresTorusGeometry :args="[0.5, 0.2, 32, 100]"   />
    <TresMeshPhongMaterial color="orange" />
  </TresMesh>
</template>