<script lang="ts" setup>
interface Project {
  name: string;
  description: string;
  skills: string[];
  links: {
    source?: string;
    release?: string;
  };
}

const projects: Project[] = [
  {
    name: "Graphics Engine",
    description:
      "I devised a rudimentary graphics rendering engine for three-dimensional geometry and established support for various texture maps, including diffusion and specular maps. I am currently working on implementing the ability to load models into the engine.",
    skills: ["C++", "OpenGL", "GLFW", "GLAD", "GLM", "GLSL"],
    links: {
      source: "https://github.com",
    },
  },
  {
    name: "Character Recognition",
    description:
      "I created a deep learning model to recognize handwritten digits and numbers using a convolution neural network. I also integrated a dropout layer to reduce overfitting.",
    skills: ["Python", "TensorFlow", "NumPy ", "Matplotlib"],
    links: {
      source: "https://github.com",
    },
  },
  {
    name: "ARM Processor",
    description:
      "I constructed a processor using the ARM instruction set architecture that supports arithmetic and boolean operations and various branching instructions.",
    skills: ["ARM", "DS-5", "Verilog", "Vivado"],
    links: {
      source: "https://github.com",
    },
  },
  {
    name: "Content Archive",
    description:
      "I developed a secure web and desktop application that manages various content types using cloud and local storage.",
    skills: [
      "TypeScript",
      "VueJS",
      "NuxtJS",
      "Element",
      "CSS",
      "TailwindCSS",
      "HTML",
      "PostgreSQL",
      "Supabase",
    ],
    links: {
      source: "https://github.com",
    },
  },
];
const incomplete: Project[] = [
  {
    name: "Portfolio Website",
    description: "",
    skills: [
      "TypeScript",
      "VueJS",
      "NuxtJS",
      "ThreeJS",
      "GLSL",
      "CSS",
      "TailwindCSS",
      "HTML",
    ],
    links: {
      source: "https://github.com",
    },
  },
];
</script>

<template>
  <PrimitiveSection title="PROJECTS">
    <div class="text-lg">
      <div v-for="project in projects" v-bind:key="project.name">
        <div class="font-bold">{{ project.name }}</div>
        <div class="">{{ project.description }}</div>
        <div class="text-sm">
          <div
            v-for="skill in project.skills"
            class="inline-flex mx-0.5 my-0.5 px-1.5 py-0.5 border-2 rounded-md border-white border-opacity-50 text-white-3"
          >
            {{ skill }}
          </div>
        </div>
      </div>
    </div>
  </PrimitiveSection>
</template>

<style scoped></style>
