<template>
  <div>
    {{ data }}
  </div>
</template>

<script setup>
const props = defineProps({
  data: {
    type: Array,
    default: () => [],
  }
})
</script>

<style lang="scss" scoped>

</style>
