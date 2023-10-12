<script lang="ts" setup></script>

<template>
  <div class="flex flex-col w-full h-full lg:flex-row">
    <div
      class="top-0 flex flex-col max-h-screen lg:items-center lg:w-1/2 lg:px-9 lg:py-48 lg:sticky"
    >
      <SectionOne />
      <SectionTwo />
    </div>
    <div class="top-0 flex flex-col min-h-screen lg:items-center lg:w-1/2 lg:px-9 lg:py-24">
      <SectionThree />
      <SectionFour />
      <SectionFive />
      <SectionSix />
      <SectionSeven />
    </div>
  </div>
</template>

<style scoped></style>
