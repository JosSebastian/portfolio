<script lang="ts" setup></script>

<template>
  <div class="flex flex-col w-full h-full lg:flex-row">
    <div
      class="top-0 flex flex-col justify-between max-h-screen p-5 lg:w-1/2 lg:p-10 lg:sticky lg:items-center">
      <SectionOne />
      <SectionTwo />
    </div>
    <div
      class="top-0 flex flex-col min-h-screen justify-normal lg:w-1/2 lg:p-10">
      <SectionThree />
      <SectionFour />
      <SectionFive />
    </div>
  </div>
</template>

<style scoped></style>
