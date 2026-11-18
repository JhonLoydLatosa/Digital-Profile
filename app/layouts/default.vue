
<template>
  <div class="site-background min-h-screen overflow-hidden">
    <SiteNavbar />

    <main>
      <slot />
    </main>

    <footer class="border-t border-white/10 bg-[#101827]/70 px-6 py-8 backdrop-blur-xl md:px-12">
      <div class="mx-auto flex max-w-7xl flex-wrap items-center justify-between gap-4">
        <p class="text-xs tracking-wide text-slate-400">
          © 2026 Jhon Loyd Latosa. ALL RIGHTS RESERVED.
        </p>

        <p class="text-xs text-slate-500">
          Made with creativity and curiosity.
        </p>
      </div>
    </footer>
  </div>
</template>
