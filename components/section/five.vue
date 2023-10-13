<script lang="ts" setup>
interface Experience {
  time: {
    start: string;
    end: string;
  };
  position: string;
  company: string;
  description: string;
  skills: string[];
}
const experiences: Experience[] = [
  {
    time: {
      start: "2021",
      end: "Current",
    },
    position: "Mathematics Tutor",
    company: "Texas A&M University",
    description:
      "As a Mathematics Tutor at Texas A&M University's Academic Success Center, I foster my students' understanding of various math concepts from pre-algebra to pre-calculus. I work closely with each student group to create a customized lesson plan that caters to their learning style and pace. I also took the responsibility of maintaining and updating the online course page, ensuring that it provides students with relevant content to support their academic careers.",
    skills: [],
  },
];
</script>

<template>
  <PrimitiveSection title="EXPERIENCE">
    <div class="text-lg">
      <div
        v-for="experience in experiences"
        v-bind:key="experience.company"
        class="flex gap-3"
      >
        <div>
          <span>{{ experience.time.start }} - {{ experience.time.end }}</span>
        </div>
        <div>
          <div class="font-bold">
            {{ experience.position }} - {{ experience.company }}
          </div>
          <div class="">{{ experience.description }}</div>
          <div class="text-sm">
            <div v-for="skill in experience.skills" class="inline-block">
              {{ skill }}
            </div>
          </div>
        </div>
      </div>
    </div>
  </PrimitiveSection>
</template>

<style scoped></style>
