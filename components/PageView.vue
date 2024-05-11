<script setup lang="ts">
const { data } = await useFetch('/api/pageview')

const time = useTimeAgo(() => data.value?.startAt || 0)
</script>

<template>
  <div text-gray:80>
    <span text-gray font-500>{{ data?.pageview }}</span>
    page views since1111111111111111111111
    <span text-gray>{{ time }}</span>
  </div>
</template>
