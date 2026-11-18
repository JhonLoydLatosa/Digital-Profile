
<script setup>
useHead({
  title: 'About Me | Jhon Loyd Latosa',
  meta: [
    {
      name: 'description',
      content: 'Learn more about my background, education, skills, and interests.'
    }
  ]
})

const personalInfo = [
  { label: 'FULL NAME', value: 'Jhon Loyd Latosa' },
  { label: 'AGE', value: '20' },
  { label: 'LOCATION', value: 'Butuan city, Philippines' },
  { label: 'COURSE', value: 'BS Information Technology' },
  { label: 'YEAR LEVEL', value: 'Third Year' },
  { label: 'COLLEGE/UNIVERSITY', value: 'Caraga State University - Main Campus' }
]

const skills = [
  { name: 'HTML', level: 'Basic/Fundamentals' },
  { name: 'CSS', level: 'Basic/Fundamentals' },
  { name: 'JavaScript', level: 'Inprogress' },
  { name: 'Vue.js', level: 'Inprogress' },
  { name: 'Nuxt.js', level: 'Inprogress' },
  { name: 'Tailwind CSS', level: 'Inprogress' }
]

const interests = [
  'Frontend Development',
  'UI/UX Design',
  'Web Technologies',
  'Creative Design'
]

const hobbies = [
  'Playing Online Games',
  'Listening to Music',
  'Watching Movies',
  'Exploring New Technologies'
]
</script>

<template>
  <div class="text-[#F1F5F9]">

    
    <!-- PROFILE INTRO -->
    <section class="profile-hero relative isolate px-6 py-24 md:px-12 md:py-32">

    <!-- DECORATIVE BACKGROUND LAYER -->
    <div class="absolute inset-0 z-0 pointer-events-none" aria-hidden="true">
        <div class="particle-field">
        <span v-for="n in 6" :key="n" class="particle"></span>
        </div>

        <!-- Orb stays behind the text -->
        <div class="orb-decoration profile-hero-orb">
        <div class="orb-ring"></div>
        <div class="orb-ring-secondary"></div>
        <div class="glass-orb"></div>
        <span class="orb-mini orb-mini-one"></span>
        <span class="orb-mini orb-mini-two"></span>
        <span class="orb-mini orb-mini-three"></span>
        </div>
    </div>

    <!-- ACTUAL CONTENT: ALWAYS IN FRONT -->
    <div class="relative z-10 mx-auto max-w-7xl">

        <p class="text-xs font-semibold tracking-[0.2em] text-blue-300">
        A CLOSER LOOK AT ME
        </p>

        <h1 class="mt-7 text-5xl font-extrabold leading-tight sm:text-7xl">
        GET TO KNOW
        <span class="block bg-gradient-to-r from-blue-300 to-slate-300 bg-clip-text text-transparent">
            ME BETTER.
        </span>
        </h1>

        <p class="mt-7 max-w-2xl leading-8 text-slate-400">
        A little introduction to my background, educational journey,
        interests, skills, and the things that make me who I am.
        </p>

    </div>
    </section>

    <!-- PERSONAL INFORMATION -->
    <section class="relative z-10 px-6 py-20 md:px-12">
      <div class="mx-auto max-w-7xl">
        <p class="text-xs font-semibold tracking-[0.2em] text-blue-300">
          01 / PERSONAL DETAILS
        </p>

        <h2 class="mt-4 text-3xl font-bold">
          Personal Information
        </h2>

        <div class="mt-10 grid gap-4 sm:grid-cols-2 lg:grid-cols-3">
          <article
            v-for="(item, index) in personalInfo"
            :key="item.label"
            class="glass-card rounded-2xl p-6"
          >
            <p class="text-xs tracking-widest text-blue-300">
              {{ item.label }}
            </p>

            <p class="mt-4 text-lg font-semibold text-white">
              {{ item.value }}
            </p>

          </article>
        </div>
      </div>
    </section>

    <!-- EDUCATION -->
    <section class="relative overflow-hidden px-6 py-24 md:px-12">
      <div class="absolute inset-0 bg-gradient-to-b from-[#1E293B]/55 to-transparent"></div>

      <div class="relative mx-auto max-w-7xl">
        <p class="text-xs font-semibold tracking-[0.2em] text-blue-300">
          02 / EDUCATION
        </p>

        <h2 class="mt-4 text-3xl font-bold">
          My Learning Journey
        </h2>

        <div class="glass-panel mt-10 rounded-3xl p-8 md:p-10">
          <p class="text-sm font-medium text-blue-300">
            2024 — PRESENT
          </p>

          <h3 class="mt-5 text-2xl font-bold text-white">
            Bachelor of Science in Information Technology
          </h3>

          <p class="mt-3 text-slate-300">
            Caraga State University - Main campus
          </p>

          <p class="mt-5 max-w-2xl text-sm leading-8 text-slate-400">
            I am currently pursuing a degree in Information Technology,
            where I continue to develop my knowledge of programming,
            software development, web technologies, and computer systems.
          </p>
        </div>
      </div>
    </section>

    <!-- SKILLS -->
    <section class="px-6 py-24 md:px-12">
      <div class="mx-auto max-w-7xl">
        <p class="text-xs font-semibold tracking-[0.2em] text-blue-300">
          03 / SKILLS & TECHNOLOGIES
        </p>

        <h2 class="mt-4 text-3xl font-bold">
          Things I'm Learning
        </h2>

        <p class="mt-4 max-w-xl leading-8 text-slate-400">
          These are some of the technologies and tools I am exploring
          as I continue developing my skills.
        </p>

        <div class="mt-10 grid gap-4 sm:grid-cols-2 lg:grid-cols-3">
          <article
            v-for="skill in skills"
            :key="skill.name"
            class="glass-card rounded-2xl p-6"
          >
            <div class="flex items-center justify-between">
              <h3 class="text-lg font-semibold text-white">
                {{ skill.name }}
              </h3>

              <span class="text-blue-300">✦</span>
            </div>

            <p class="mt-4 text-xs text-slate-400">
              {{ skill.level }}
            </p>
          </article>
        </div>
      </div>
    </section>

    <!-- INTERESTS AND HOBBIES -->
    <section class="relative overflow-hidden px-6 py-24 md:px-12">
      <div class="absolute inset-0 bg-gradient-to-b from-[#1E293B]/55 to-transparent"></div>

      <div class="relative mx-auto max-w-7xl">
        <p class="text-xs font-semibold tracking-[0.2em] text-blue-300">
          04 / BEYOND THE CLASSROOM
        </p>

        <h2 class="mt-4 text-3xl font-bold">
          More About Me
        </h2>

        <div class="mt-10 grid gap-6 md:grid-cols-2">
          <div class="glass-panel rounded-3xl p-8">
            <h3 class="text-xl font-bold text-white">
              My Interests
            </h3>

            <div class="mt-7 space-y-3">
              <div
                v-for="interest in interests"
                :key="interest"
                class="flex items-center justify-between border-b border-white/10 py-4"
              >
                <span class="text-slate-300">{{ interest }}</span>
                <span class="text-blue-300">↗</span>
              </div>
            </div>
          </div>

          <div class="glass-panel rounded-3xl p-8">
            <h3 class="text-xl font-bold text-white">
              My Hobbies
            </h3>

            <div class="mt-7 space-y-3">
              <div
                v-for="hobby in hobbies"
                :key="hobby"
                class="flex items-center justify-between border-b border-white/10 py-4"
              >
                <span class="text-slate-300">{{ hobby }}</span>
                <span class="text-blue-300">↗</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- END OF PROFILE -->
    <section class="px-6 py-24 text-center md:py-32">
      <div class="orb-scene mx-auto mb-12">
        <div class="glass-orb"></div>
      </div>

      <p class="text-xs font-semibold tracking-[0.2em] text-blue-300">
        THANK YOU FOR VISITING!
      </p>

      <h2 class="mt-6 text-4xl font-bold sm:text-5xl">
        Still growing.
        <span class="block text-blue-300">Still becoming.</span>
      </h2>

      <p class="mt-6 text-slate-400">
        Every experience is another opportunity to learn.
      </p>

      <NuxtLink
        to="/"
        class="mt-9 inline-flex rounded-full border border-blue-300/30 bg-blue-400/10 px-6 py-3 font-medium text-blue-200 transition hover:-translate-y-1 hover:bg-blue-400/20"
      >
        ← Back to Homepage
      </NuxtLink>
    </section>

  </div>
</template>
