<template>
  <div class="container">
    <Renderer ref="renderer" resize="true" orbit-ctrl>
      <Camera ref="camera" :position="{ z: 100 }" :lookAt="{x: 100, y: 100, z: 100}"/>
      <Scene background="white">
        <AmbientLight color="#ffffff" :intensity="1"/>
        <Box ref="box" :position="{x: 0, y:0, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 0, y:1, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 0, y:2, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 0, y:3, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 0, y:3, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 0, y:4, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 1, y:4, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 2, y:4, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 3, y:4, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 3, y:3, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 3, y:2, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 3, y:1, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 3, y:0, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 2, y:0, z:0}">
          <ObsidianTexture />
        </Box>
        <Box ref="box" :position="{x: 1, y:0, z:0}">
          <ObsidianTexture />
        </Box>
      </Scene>
    </Renderer>
  </div>
</template>

<script setup>
import { Renderer, Camera, Scene, PointLight, Box, LambertMaterial, AmbientLight, BasicMaterial, Texture, CubeTexture } from 'troisjs'
import ObsidianTexture from "./components/ObsidianTexture";

const renderer = ref(null)
const box = ref(null)
const camera = ref(null)

</script>

<style lang="scss">

html {
  box-sizing: border-box;
}

*, *::before, *::after{
  box-sizing: inherit;
  margin: 0;
  padding: 0;
}

.container {
  background-color: red;
  width: 100vw;
  height: 100vh;
}

</style>