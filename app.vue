<script setup lang="ts">
import { appName } from '~/constants'

useHead({
  title: appName,
})


const layout='home'
</script>

<template>
  <VitePwaManifest />
  <NuxtLayout :name="layout">
    <NuxtPage />
  </NuxtLayout>
</template>

<style>
html,
body,
#__nuxt {
  height: 100vh;
  margin: 0;
  padding: 0;
}

html.dark {
  background: #222;
  color: white;
}
</style>
