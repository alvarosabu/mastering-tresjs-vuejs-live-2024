<template>
  <TresMesh :position="[-4, 0, 0]">
    <TresTorusKnotGeometry :args="[0.5, 0.2, 64, 100]"   />
    <TresMeshNormalMaterial />
  </TresMesh>
</template>