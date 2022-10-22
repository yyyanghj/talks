<script lang="ts" setup>
import { ref, onMounted } from 'vue'
import mediumZoom from "medium-zoom";

const el = ref<HTMLImageElement | null>()

onMounted(() => {
  mediumZoom(el.value!)
})

</script>

<template>
  <img ref="el" />
</template>


<style lang="postcss" scoped>

</style>