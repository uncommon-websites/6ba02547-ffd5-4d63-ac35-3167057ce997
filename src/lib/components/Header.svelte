<script lang="ts">
  export let transparent = false;
</script>

<header class="fixed top-0 left-0 w-full z-50 transition-colors duration-300 {transparent ? 'bg-transparent text-white' : 'bg-white text-black'}">
  <div class="max-w-[1400px] mx-auto px-6 h-16 flex items-center justify-between">
    <!-- Left Navigation -->
    <nav class="flex items-center gap-8 text-[13px] font-medium tracking-wide">
      <a href="/" class="hover:opacity-70 transition-opacity">Technology</a>
      <a href="/" class="hover:opacity-70 transition-opacity">Products</a>
      <a href="/" class="hover:opacity-70 transition-opacity">Industries</a>
      <a href="/" class="hover:opacity-70 transition-opacity">Company</a>
    </nav>

    <!-- Center Logo -->
    <div class="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2">
      <a href="/" class="flex items-center">
        <svg width="45" height="57" viewBox="0 0 90 115" fill="none" xmlns="http://www.w3.org/2000/svg" class="{transparent ? 'text-white' : 'text-black'}">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M31.8701 9.95388L15.3109 19.4791L31.8819 29.0064L48.446 19.4812L31.8701 9.95388ZM53.2588 27.7795L36.6927 37.3058L36.6911 56.3603L53.2588 46.8319V27.7795ZM58.0696 55.1313L41.5014 64.66L58.072 74.187L74.6383 64.6605L58.0696 55.1313ZM79.4486 72.9601L62.883 82.4862V101.538L79.4486 92.0122V72.9601ZM53.2614 101.539V82.4864L36.6903 72.9591V92.012L53.2614 101.539ZM27.0694 56.3613L10.5003 46.8319V27.7788L27.0711 37.3058L27.0694 56.3613ZM27.0687 67.4269L4.48643 54.4394C2.25391 53.1554 0.878662 50.7828 0.878662 48.215V19.4801C0.878662 17.7684 1.79538 16.1867 3.28356 15.3307L28.2608 0.963381C30.4933 -0.320696 33.2439 -0.321154 35.4766 0.962171L60.474 15.3299C61.963 16.1857 62.8804 17.7679 62.8804 19.4801V46.8319L86.665 60.5111C88.1535 61.3671 89.0702 62.9489 89.0702 64.6607V93.3956C89.0702 95.9635 87.6948 98.3361 85.4621 99.62L60.4776 113.988C58.9894 114.843 57.1558 114.843 55.6673 113.988L30.6773 99.6202C28.4444 98.3365 27.0687 95.9635 27.0687 93.3954V67.4269Z" fill="currentColor"/>
        </svg>
      </a>
    </div>

    <!-- Right placeholder (empty in screenshot) -->
    <div class="hidden md:block w-[300px]"></div>
  </div>
</header>
