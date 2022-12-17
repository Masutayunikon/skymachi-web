<template>
  <BasicMaterial>
    <Texture ref="obsidianTexture" refraction :refraction-ratio="0.95" src="/block/obsidian.png" />
  </BasicMaterial>
</template>

<script setup>
import { BasicMaterial, Texture } from 'troisjs'
import * as THREE from "three";

const obsidianTexture = ref(null)

onMounted(() => {
  const t = obsidianTexture.value
  t.texture.magFilter = THREE.NearestFilter;
  t.texture.minFilter = THREE.NearestFilter;
})

</script>

<style scoped>

</style>