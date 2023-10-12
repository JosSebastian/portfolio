<script lang="ts" setup></script>

<template>
  <div class="flex flex-col w-full h-full lg:flex-row">
    <div
      class="top-0 flex flex-col justify-between max-h-screen p-5 lg:w-1/2 lg:px-9 lg:py-24 lg:sticky lg:items-center">
      <SectionOne />
      <SectionTwo />
    </div>
    <div
      class="top-0 flex flex-col items-center min-h-screen lg:w-1/2 lg:px-18 lg:py-24 lg:gap-12">
      <SectionThree />
      <SectionFour />
      <SectionFive />
      <SectionSix />
      <SectionSeven />
    </div>
  </div>
</template>

<style scoped></style>
