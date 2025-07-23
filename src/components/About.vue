<template>
  <section id="about" class="py-16 sm:py-20 bg-gradient-to-b from-gray-900 to-blue-900">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Heading -->
      <h2
        v-intersect
        class="text-3xl sm:text-4xl font-bold text-white text-center opacity-0 translate-y-4 transition duration-700"
      >
        About Me
      </h2>

      <!-- Intro -->
      <p
        v-intersect
        class="mt-6 text-lg text-gray-300 max-w-3xl mx-auto text-center opacity-0 translate-y-4 transition duration-700 delay-200"
      >
        I’m <strong>Mercy Chepngeno</strong>, a software Engineer with
         a passion for polished, well‑documented projects. I thrive in collaborative,
        growth‑oriented environments and am open to roles where I can help build
        accessible, impactful web experiences.
      </p>

      <!-- Experience -->
      <div class="mt-12">
        <h3
          v-intersect
          class="text-2xl font-semibold text-orange-500 text-center opacity-0 translate-y-4 transition duration-700 delay-400"
        >
          Experience
        </h3>
        <div class="mt-6 space-y-6">
          <!-- Facility Hub -->
          <div
            v-intersect
            class="bg-gray-800 p-6 rounded-lg shadow-md hover:shadow-orange-500/50 transition opacity-0 -translate-x-4 transition duration-700 delay-500"
          >
            <h4 class="text-xl font-semibold text-white">
              Software Developer Volunteer, Facility Hub
            </h4>
            <p class="text-gray-300">2025 – Present</p>
            <ul class="mt-2 text-gray-300 list-disc list-inside space-y-1">
              <li>Developed a fullstack web modules using Vue.js and Node.js, accounting for ~60% of the platform’s user-facing components and logic, including authentication and dashboard features.</li>
              <li>Integrated RESTful APIs and optimized MySQL queries, contributing to a 40% improvement in data retrieval performance and faster UI responsiveness across devices.</li>
              <li>Engineered reusable components and implemented routing logic, enabling 50% faster feature development cycles and reducing maintenance effort.</li>
              <li>Collaborated cross-functionally with a remote team, driving ~30% of feature delivery from ideation to production by actively shaping technical requirements and implementation plans.</li>
            </ul>
          </div>

          <!-- Moran Publishers -->
          <div
            v-intersect
            class="bg-gray-800 p-6 rounded-lg shadow-md hover:shadow-orange-500/50 transition opacity-0 translate-x-4 transition duration-700 delay-600"
          >
            <h4 class="text-xl font-semibold text-white">
              Software Developer, Moran Publishers
            </h4>
            <p class="text-gray-300">2022 – 2024</p>
            <ul class="mt-2 text-gray-300 list-disc list-inside space-y-1">
              <li>Built dynamic web features using React and TypeScript, delivering ~70% of new product-facing modules including blog displays, admin dashboards, and content filtering logic.</li>
              <li>Maintained and extended a custom CMS built with Python Django, contributing to ~50% of backend enhancements such as editorial workflows, publishing permissions, and asset management</li>
              <li>Improved UI/UX across key pages using Tailwind CSS, leading to ~35% faster page load times and a 20% increase in user engagement based on internal analytics.</li>
              <li>Collaborated with editors and designers to implement pixel-perfect components, reducing iteration cycles by ~40% and accelerating feature sign-offs.</li>
            </ul>
          </div>
        </div>
      </div>

      <!-- Education -->
      <div class="mt-12">
        <h3
          v-intersect
          class="text-2xl font-semibold text-orange-500 text-center opacity-0 translate-y-4 transition duration-700 delay-700"
        >
          Education
        </h3>
        <div
          v-intersect
          class="mt-6 bg-gray-800 p-6 rounded-lg shadow-md hover:shadow-orange-500/50 transition opacity-0 translate-y-4 transition duration-700 delay-800"
        >
          <h4 class="text-xl font-semibold text-white">
            Bachelor of Science in Computer Science
          </h4>
          <p class="text-gray-300">
            Catholic University of Eastern Africa, 2018 – 2024
          </p>
          <p class="mt-2 text-gray-300">
            Focused on software engineering, problem solving, and fullstack web
            development.
          </p>
        </div>
      </div>

      <!-- Skills -->
      <div class="mt-12">
        <h3
          v-intersect
          class="text-2xl font-semibold text-orange-500 text-center opacity-0 translate-y-4 transition duration-700 delay-900"
        >
          Skills
        </h3>
        <div class="mt-6 grid gap-6 sm:grid-cols-2 lg:grid-cols-3">
          <div
            v-for="(skill, i) in skills"
            :key="skill.name"
            v-intersect
            class="bg-gray-800 p-6 rounded-lg shadow-md hover:shadow-orange-500/50 hover:scale-105 transition opacity-0 translate-y-4 transition duration-700"
            :class="`delay-${200 + i * 100}`"
          >
            <span class="text-2xl text-orange-500">{{ skill.icon }}</span>
            <p class="mt-2 text-lg font-semibold text-white">{{ skill.name }}</p>
          </div>
        </div>
      </div>

      <!-- Call to Action -->
      <div
        v-intersect
        class="mt-12 text-center opacity-0 translate-y-4 transition duration-700 delay-1200"
      >
        <p class="text-lg text-gray-200">
          🚀 <strong>Actively seeking software engineer roles.</strong><br />
          Connect with me on
          <a
            href="https://github.com/chep-collab"
            target="_blank"
            class="text-orange-400 underline"
            >GitHub</a
          > or
          <a
            href="https://www.linkedin.com/in/mercy-chepngeno-48b72920a/"
            target="_blank"
            class="text-orange-400 underline"
            >LinkedIn</a
          >.
        </p>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'

const skills = ref([
  { name: 'Vue.js', icon: '🖌️' },
  { name: 'React', icon: '⚛️' },
  { name: 'TypeScript', icon: '📜' },
  { name: 'Node.js', icon: '🟢' },
  { name: 'MySQL', icon: '🗄️' },
  { name: 'REST APIs', icon: '🌐' },
  { name: 'GraphQL', icon: '📊' },
  { name: 'Tailwind CSS', icon: '🎨' },
  { name: 'Git', icon: '🐙' },
  { name: 'Docker', icon: '🐳' },
  { name: 'CI/CD', icon: '🔄' },
  { name: 'Python Django', icon: '🚀' },
  { name: '.NET', icon: '🎯' },
  { name: 'Agile', icon: '📈' },
  { name: 'Problem Solving', icon: '🧩' }
])
</script>
