
<script setup>
useHead({
  title: 'Jhon Loyd Latosa | Digital Profile',
  meta: [
    {
      name: 'description',
      content: 'A personal portfolio sharing my background, interests, and learning journey.'
    }
  ]
})

const technologies = [
  'HTML',
  'CSS',
  'JavaScript',
  'Vue.js',
  'Nuxt.js',
  'Tailwind CSS'
]

const snapshots = [
  {
    number: '01',
    title: 'Education',
    description: 'Third-Year IT Student',
    detail: 'Caraga State University - Main Campus'
  },
  {
    number: '02',
    title: 'Interests',
    description: 'Development & Design',
    detail: 'Exploring creative technologies'
  },
  {
    number: '03',
    title: 'Mindset',
    description: 'Always Improving',
    detail: 'Learning something new every day'
  }
]
</script>

<template>
  <div class="text-[#F1F5F9]">

    <!-- HOMEPAGE HERO -->
    <section class="relative isolate overflow-hidden px-6 py-20 md:px-12 md:py-28">

      <!-- Floating particles -->
      <div class="particle-field" aria-hidden="true">
        <span v-for="n in 6" :key="n" class="particle"></span>
      </div>

      <div class="relative z-10 mx-auto grid max-w-7xl items-center gap-16 lg:grid-cols-[1.15fr_0.85fr]">

        <!-- INTRODUCTION -->
        <div>
          <div class="mb-8 inline-flex items-center gap-3 rounded-full border border-blue-300/20 bg-blue-400/10 px-4 py-2 backdrop-blur-md">
            <span class="h-2 w-2 rounded-full bg-blue-400"></span>
            <span class="text-xs font-medium tracking-wide text-blue-200">
              WELCOME TO MY PERSONAL SPACE
            </span>
          </div>

          <p class="mb-4 text-sm font-medium tracking-[0.2em] text-blue-300">
            HELLO, I'M
          </p>

          <h1 class="text-5xl font-extrabold leading-[1.08] tracking-tight sm:text-7xl">
            Jhon Loyd
            <span class="block bg-gradient-to-r from-blue-300 to-slate-300 bg-clip-text text-transparent">
              Latosa
            </span>
          </h1>

          <h2 class="mt-7 text-xl font-medium text-slate-200 sm:text-2xl">
            Growing, creating, and discovering new possibilities.
          </h2>

          <p class="mt-5 max-w-xl text-base leading-8 text-slate-400">
            I'm a third-year Information Technology student at Caraga State
            University - Main Campus.I enjoy learning about technology, exploring creative
            ideas, and developing my skills one step at a time.
          </p>

          <div class="mt-9 flex flex-wrap gap-4">
            <NuxtLink
              to="/profile"
              class="rounded-full border border-blue-300/40 bg-blue-400 px-6 py-3.5 font-semibold text-[#101827] shadow-lg shadow-blue-500/20 transition hover:-translate-y-1 hover:bg-blue-300"
            >
              Explore My Profile ↗
            </NuxtLink>

            <a
              href="mailto:your-email@example.com"
              class="rounded-full border border-white/15 bg-white/5 px-6 py-3.5 font-medium text-slate-200 backdrop-blur-md transition hover:border-blue-300/50 hover:bg-blue-400/10"
            >
              Let's Connect
            </a>
          </div>

          <!-- TECHNOLOGY TAGS -->
          <div class="mt-12">
            <p class="mb-4 text-xs font-medium tracking-[0.18em] text-slate-500">
              CURRENTLY EXPLORING
            </p>

            <div class="flex flex-wrap gap-2">
              <span
                v-for="tech in technologies"
                :key="tech"
                class="rounded-full border border-white/10 bg-white/5 px-4 py-2 text-xs text-slate-300 backdrop-blur-md"
              >
                {{ tech }}
              </span>
            </div>
          </div>
        </div>

        
        <!-- PHOTO AND ORB -->
        <div class="relative mx-auto w-full max-w-sm">

        <!-- Soft blue glow behind everything -->
        <div
            class="blue-glow absolute inset-0 z-0 scale-90 rounded-full"
            aria-hidden="true"
        ></div>

        <!-- OPTION 6: ORBITAL 3D WITH PARTICLES -->
        <div class="orb-decoration" aria-hidden="true">

            <!-- Orbital rings -->
            <div class="orb-ring"></div>
            <div class="orb-ring-secondary"></div>

            <!-- Main glass sphere -->
            <div class="glass-orb"></div>

            <!-- Floating mini spheres -->
            <span class="orb-mini orb-mini-one"></span>
            <span class="orb-mini orb-mini-two"></span>
            <span class="orb-mini orb-mini-three"></span>

        </div>

        <!-- PROFILE PHOTO: ALWAYS IN FRONT -->
        <div
            class="profile-3d relative z-10 aspect-[4/5] w-full overflow-hidden rounded-[2rem] border border-blue-200/30 bg-[#1E293B]"
        >

            <img
            src="/images/llourd.jpg"
            alt="My profile photo"
            class="absolute inset-0 h-full w-full object-cover object-[center_35%]"
            />

            <!-- Soft glass overlay -->
            <div
            class="pointer-events-none absolute inset-0 bg-gradient-to-t from-[#101827]/55 via-transparent to-white/10"
            ></div>

            <!-- Current status glass card -->
            <div class="glass-panel absolute bottom-4 left-4 z-10 rounded-xl px-4 py-3">
            <p class="text-[10px] tracking-widest text-blue-200">
                CURRENT STATUS
            </p>
            <p class="mt-1 text-sm font-semibold text-white">
                IT Student
            </p>
            </div>

            <!-- Code decoration -->
            <div class="absolute bottom-4 right-4 z-20 rounded-lg border border-blue-300/30 bg-[#101827]/85 px-3 py-2 font-mono text-xs text-blue-300">
            &lt;/&gt;
            </div>

        </div>

        <!-- Caption -->
        <p class="relative z-10 mt-6 text-center text-xs tracking-widest text-slate-500">
            A LITTLE INTRODUCTION ABOUT ME
        </p>

        </div>
      </div>
    </section>

    <!-- INTRODUCTION SECTION -->
    <section class="relative px-6 py-24 md:px-12">
      <div class="particle-field opacity-40" aria-hidden="true">
        <span v-for="n in 6" :key="n" class="particle"></span>
      </div>

      <div class="relative mx-auto grid max-w-7xl gap-12 md:grid-cols-2">

        <div>
          <p class="text-xs font-semibold tracking-[0.2em] text-blue-300">
            A LITTLE ABOUT MYSELF
          </p>

          <h2 class="mt-5 text-4xl font-bold leading-tight sm:text-5xl">
            More than just
            <span class="text-blue-300">a student.</span>
          </h2>
        </div>

        <div class="flex flex-col justify-end">
          <p class="leading-8 text-slate-400">
            Welcome to my personal space! This website is a reflection of who
            I am, what I enjoy, and what I continue to learn. Here, you can
            explore my educational background, skills, interests, and
            experiences as I work toward my goals.
          </p>

          <NuxtLink
            to="/profile"
            class="mt-8 inline-flex items-center justify-between border-b border-white/15 py-5 text-sm font-semibold text-blue-300 transition hover:border-blue-300"
          >
            GET TO KNOW ME
            <span class="text-xl">↗</span>
          </NuxtLink>
        </div>
      </div>
    </section>

    <!-- GLASS SNAPSHOT CARDS -->
    <section class="relative overflow-hidden px-6 py-24 md:px-12">
      <div class="absolute inset-0 bg-gradient-to-b from-[#1E293B]/40 to-transparent"></div>

      <div class="relative mx-auto max-w-7xl">
        <p class="text-xs font-semibold tracking-[0.2em] text-blue-300">
          A QUICK LOOK AT MY JOURNEY
        </p>

        <h2 class="mt-5 text-3xl font-bold sm:text-4xl">
          A few things about me
        </h2>

        <div class="mt-12 grid gap-5 md:grid-cols-3">
          <article
            v-for="item in snapshots"
            :key="item.number"
            class="glass-card rounded-3xl p-7"
          >
            <div class="flex items-center justify-between">
              <span class="text-sm font-medium text-blue-300">
                {{ item.number }}
              </span>
              <span class="h-2 w-2 rounded-full bg-blue-300 shadow-[0_0_12px_#60A5FA]"></span>
            </div>

            <h3 class="mt-9 text-sm text-slate-400">
              {{ item.title }}
            </h3>

            <p class="mt-2 text-xl font-bold text-white">
              {{ item.description }}
            </p>

            <p class="mt-3 text-sm leading-6 text-slate-400">
              {{ item.detail }}
            </p>
          </article>
        </div>
      </div>
    </section>

    <!-- TECHNOLOGY INTEREST -->
    <section class="px-6 py-24 md:px-12">
      <div class="glass-panel mx-auto max-w-7xl rounded-[2rem] p-8 md:p-14">
        <div class="grid items-center gap-12 md:grid-cols-[1fr_auto]">
          <div>
            <p class="text-xs font-semibold tracking-[0.2em] text-blue-300">
              WHAT I'M EXPLORING
            </p>

            <h2 class="mt-5 text-3xl font-bold sm:text-4xl">
              Curious about what's possible.
            </h2>

            <p class="mt-5 max-w-xl leading-8 text-slate-400">
              I'm interested in discovering new tools, improving my
              technical knowledge, and creating digital experiences
              that are useful and meaningful.
            </p>
          </div>

          <div class="orb-scene mx-auto">
            <div class="orb-ring"></div>
            <div class="glass-orb"></div>
          </div>
        </div>
      </div>
    </section>

  </div>
</template>
