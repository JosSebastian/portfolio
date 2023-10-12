<script lang="ts" setup>
const { title } = defineProps<{ title?: string }>();
</script>

<template>
  <div class="p-3 m-0">
    <div v-if="title" class="top-0 text-xl font-semibold">
      {{ title }}
    </div>
    <slot />
  </div>
</template>

<style scoped></style>
