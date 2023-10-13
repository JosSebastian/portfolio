<script lang="ts" setup>
interface Skill {
  category: string;
  skills: {
    name: string;
    subskills?: string[];
    tools?: string[];
  }[];
}
const skills: Skill[] = [
  {
    category: "Languages",
    skills: [
      {
        name: "C++",
        subskills: ["OpenGL", "GLFW", "ImGui"],
        tools: ["CMake", "Valgrind", "GDB"],
      },
      {
        name: "Python",
        subskills: ["PyTorch", "Pandas", "NumPy", "Matplotlib"],
        tools: ["Jupyter"],
      },
    ],
  },
];
</script>

<template>
  <PrimitiveSection title="SKILLS"> </PrimitiveSection>
</template>

<style scoped></style>
