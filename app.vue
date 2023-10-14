<script setup lang="ts">
useHead({
  title: "Jos Sebastian",
  meta: [
    {
      name: "description",
      content: "Portfolio",
    },
  ],
  link: [
    {
      rel: "icon",
      type: "image/x-icon",
      href: "/fav.ico",
    },
  ],
});
</script>

<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
