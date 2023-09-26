<script lang="ts" setup>
const { title } = defineProps<{ title?: string }>();
</script>

<template>
  <div>
    <div
      v-if="title"
      class="sticky top-0 px-5 py-5 text-xl font-semibold lg:hidden backdrop-blur">
      {{ title }}
    </div>
    <slot />
  </div>
</template>

<style scoped></style>
