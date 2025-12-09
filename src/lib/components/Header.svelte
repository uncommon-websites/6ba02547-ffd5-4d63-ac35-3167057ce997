<script lang="ts">
  export let transparent = false;
</script>

<header class="fixed top-0 left-0 w-full z-50 transition-colors duration-300 {transparent ? 'bg-transparent text-white' : 'bg-white text-black'}">
  <div class="max-w-[1400px] mx-auto px-6 h-16 flex items-center justify-between">
    <!-- Left Navigation -->
    <nav class="flex items-center gap-8 text-[13px] font-medium tracking-wide">
      <a href="/" class="hover:opacity-70 transition-opacity">Technology</a>
      <a href="/" class="hover:opacity-70 transition-opacity">AIRMADE® SAF</a>
      <a href="/" class="hover:opacity-70 transition-opacity">Defense</a>
      <a href="/" class="hover:opacity-70 transition-opacity">Company</a>
    </nav>

    <!-- Center Logo -->
    <div class="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2">
      <a href="/" class="text-2xl font-bold tracking-widest uppercase font-sans">AIRCO</a>
    </div>

    <!-- Right placeholder (empty in screenshot) -->
    <div class="hidden md:block w-[300px]"></div>
  </div>
</header>
