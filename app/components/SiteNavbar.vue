
<script setup>
const route = useRoute()

const links = [
  { name: 'Home', path: '/' },
  { name: 'Profile', path: '/profile' }
]
</script>

<template>
  <header class="sticky top-0 z-50 border-b border-white/10 bg-[#101827]/80 px-5 backdrop-blur-xl md:px-12">
    <nav class="mx-auto flex max-w-7xl items-center justify-between py-4">

      <!-- LEFT: LOGO -->
      <NuxtLink to="/" class="flex shrink-0 items-center gap-3">
        <div class="flex h-10 w-10 items-center justify-center rounded-xl border border-blue-300/30 bg-blue-400/10 font-bold text-blue-300 shadow-lg shadow-blue-500/10">
          LV
        </div>

        <span class="font-bold tracking-wide text-white">
          lvbllourd<span class="text-blue-400">.dev</span>
        </span>
      </NuxtLink>

      <!-- RIGHT: NAVIGATION + DIGITAL PROFILE -->
      <div class="ml-auto flex items-center gap-5 sm:gap-8">

        <!-- NAVIGATION LINKS -->
        <div class="flex items-center gap-2 sm:gap-5">
          <NuxtLink
            v-for="link in links"
            :key="link.path"
            :to="link.path"
            class="rounded-full px-3 py-2 text-sm font-medium transition"
            :class="route.path === link.path
              ? 'bg-blue-400/10 text-blue-300'
              : 'text-slate-400 hover:text-white'"
          >
            {{ link.name }}
          </NuxtLink>
        </div>

        <!-- SEPARATOR -->
        <div class="hidden h-7 w-px bg-white/15 sm:block"></div>

        <!-- DIGITAL PROFILE -->
        <div class="hidden items-center gap-2 sm:flex">
          <span class="h-2 w-2 rounded-full bg-blue-400 shadow-[0_0_10px_#60A5FA]"></span>
          <span class="whitespace-nowrap text-[10px] font-medium tracking-widest text-slate-400">
            DIGITAL PROFILE
          </span>
        </div>

      </div>
    </nav>
  </header>
</template>
