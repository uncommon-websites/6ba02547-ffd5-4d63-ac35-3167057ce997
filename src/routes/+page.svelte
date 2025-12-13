<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Footer from "$lib/components/Footer.svelte";
  
  // Images
  const heroImage = "/generated/image-industrial-pipeline-with-protective-coat-1765594903929-0.webp";
  const factoryImage = "/generated/image-advanced-manufacturing-facility-with-pre-1765594906804-1.webp";
  const presentationImage = "/generated/image-materials-scientist-examining-nanomateri-1765594909821-2.webp";
  const labImage = "/generated/image-engineering-team-collaborating-on-advanc-1765594912883-3.webp";

  // Industry Partners & Government
  const partnersGov = [
    { name: "Government of Canada", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/6d/Coat_of_arms_of_Canada_rendition.svg/1200px-Coat_of_arms_of_Canada_rendition.svg.png" },
    { name: "Natural Resources Canada", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/c/c8/Natural_Resources_Canada_logo.svg/2560px-Natural_Resources_Canada_logo.svg.png" },
  ];

  const partnersIndustry = [
    { name: "Oil Sands Operations" },
    { name: "Mining Companies" },
    { name: "Petrochemical Facilities" },
    { name: "SMR Technology Partners" },
  ];

  const jobs = [
    { category: "Future Opportunities", title: "Don't see the job you're looking for? Reach out anyway", location: "Edmonton, Alberta, Canada" },
    { category: "Research & Technology", title: "Senior Materials Scientist", location: "Edmonton, Alberta, Canada" },
    { category: "Research & Technology", title: "Catalysis Research Engineer", location: "Edmonton, Alberta, Canada" },
    { category: "Research & Technology", title: "Surface Science Specialist", location: "Edmonton, Alberta, Canada" },
    { category: "Manufacturing", title: "Coating Process Engineer", location: "Edmonton, Alberta, Canada" },
    { category: "Manufacturing", title: "Advanced Manufacturing Technician", location: "Edmonton, Alberta, Canada" },
    { category: "Manufacturing", title: "Quality Assurance Manager", location: "Edmonton, Alberta, Canada" },
    { category: "Business Development", title: "Technical Sales Engineer - Oil Sands", location: "Edmonton, Alberta, Canada" },
    { category: "Business Development", title: "Business Development Manager - Mining", location: "Edmonton, Alberta, Canada" },
  ];
</script>

<Header />

<main class="font-sans text-black selection:bg-gray-200 pt-16">
  <!-- Hero Section -->
  <section class="relative h-[85vh] w-full overflow-hidden">
    <div class="absolute inset-0 bg-black/30 z-10"></div>
    <img 
      src={heroImage} 
      alt="Industrial equipment with protective coating" 
      class="w-full h-full object-cover object-center"
    />
    <div class="absolute inset-0 z-20 flex items-center justify-center">
      <h1 class="text-white text-5xl md:text-7xl font-normal text-center leading-tight max-w-4xl mx-auto px-4 drop-shadow-lg">
        Extreme Wear Protection<br />Through Nanomaterial Innovation
      </h1>
    </div>
  </section>

  <!-- Intro Section -->
  <section class="py-24 px-6 max-w-[1400px] mx-auto">
    <div class="grid grid-cols-1 md:grid-cols-12 gap-12">
      <div class="md:col-span-4">
        <h2 class="text-2xl font-normal tracking-wide mb-2 uppercase">QUANTIAM</h2>
        <p class="text-[10px] font-bold tracking-widest uppercase text-gray-500">ADVANCED MATERIALS</p>
      </div>
      <div class="md:col-span-8 grid grid-cols-1 md:grid-cols-2 gap-12 relative">
        <div class="col-span-2 md:col-span-2 space-y-6 text-[15px] leading-relaxed text-gray-800 max-w-3xl font-light">
          <p>
            Quantiam delivers extreme wear protection and low-carbon fuel production through proprietary nanomaterial coatings and advanced catalysts. Operating from Edmonton, Alberta, we house the most advanced private sector R&T and trial manufacturing capabilities in Canada.
          </p>
          <p>
            Our breakthrough technology is a global leader in non-line-of-sight deposition processes, enabling coating of internal and external surfaces of complex shapes and tubulars. This proprietary capability opens an $8B industrial coatings market, starting with critical wear protection for oil sands operations.
          </p>
          <p>
            With three platform technology families advanced to Technology Readiness Level 8—Q-XT/Gen-1 Tiles, Q-Tough Coatings, and WHm Coatings—we work across the full innovation spectrum from basic research through commercialization. Our current capacity of 1 million square inches per year is expandable to 3 million, with commercial scale operations planned for 2027.
          </p>
          <p>
            Backed by over 150 years of collective scientific and engineering experience, our Research & Technology team brings world-class expertise in catalysis, surface science, materials science, and metallurgy to solve the most demanding industrial challenges.
          </p>
        </div>
        
        <!-- Logo Mark -->
        <div class="absolute -bottom-12 right-0 hidden md:block">
           <svg width="48" height="60" viewBox="0 0 90 115" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path fill-rule="evenodd" clip-rule="evenodd" d="M31.8701 9.95388L15.3109 19.4791L31.8819 29.0064L48.446 19.4812L31.8701 9.95388ZM53.2588 27.7795L36.6927 37.3058L36.6911 56.3603L53.2588 46.8319V27.7795ZM58.0696 55.1313L41.5014 64.66L58.072 74.187L74.6383 64.6605L58.0696 55.1313ZM79.4486 72.9601L62.883 82.4862V101.538L79.4486 92.0122V72.9601ZM53.2614 101.539V82.4864L36.6903 72.9591V92.012L53.2614 101.539ZM27.0694 56.3613L10.5003 46.8319V27.7788L27.0711 37.3058L27.0694 56.3613ZM27.0687 67.4269L4.48643 54.4394C2.25391 53.1554 0.878662 50.7828 0.878662 48.215V19.4801C0.878662 17.7684 1.79538 16.1867 3.28356 15.3307L28.2608 0.963381C30.4933 -0.320696 33.2439 -0.321154 35.4766 0.962171L60.474 15.3299C61.963 16.1857 62.8804 17.7679 62.8804 19.4801V46.8319L86.665 60.5111C88.1535 61.3671 89.0702 62.9489 89.0702 64.6607V93.3956C89.0702 95.9635 87.6948 98.3361 85.4621 99.62L60.4776 113.988C58.9894 114.843 57.1558 114.843 55.6673 113.988L30.6773 99.6202C28.4444 98.3365 27.0687 95.9635 27.0687 93.3954V67.4269Z" fill="currentColor"/>
          </svg>
        </div>
      </div>
    </div>
  </section>

  <!-- Factory Image -->
  <section class="w-full px-6 pb-24 max-w-[1400px] mx-auto">
    <div class="aspect-[16/9] w-full overflow-hidden bg-gray-100">
      <img src={factoryImage} alt="Advanced Manufacturing Coatings Facility" class="w-full h-full object-cover" />
    </div>
  </section>

  <!-- Team Section -->
  <section class="py-24 px-6 max-w-[1400px] mx-auto border-t border-transparent">
    <div class="grid grid-cols-1 md:grid-cols-12 gap-12">
      <div class="md:col-span-4">
        <h2 class="text-4xl md:text-5xl font-normal tracking-tight">The Quantiam Team</h2>
      </div>
      <div class="md:col-span-8 space-y-8">
        <p class="text-[15px] leading-relaxed text-gray-800 font-light max-w-3xl">
          Our Research & Technology team brings over 150 years of collective scientific and engineering experience across catalysis, surface science, materials science, and metallurgy. We actively recruit world-class scientists, engineers, and business development specialists with expertise in NanoTechnology, Nanoscience, Nanometrics, Nanopowders, Tribology, Surface Science, Catalysis, Materials Science, Physical Chemistry, and High Temperature Manufacturing Technologies. Together, we're advancing the most extensive Advanced Materials development and characterization facilities in Canada's private sector.
        </p>
        <button class="bg-black text-white px-6 py-2 rounded-full text-[11px] font-bold uppercase tracking-widest hover:bg-gray-800 transition-colors">
          View Open Positions
        </button>
      </div>
    </div>
  </section>

  <!-- Dual Images -->
  <section class="w-full px-6 pb-24 max-w-[1400px] mx-auto">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <div class="aspect-[3/4] bg-gray-200 overflow-hidden relative group">
        <img src={presentationImage} alt="Materials scientist examining nanomaterial coating" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
        <div class="absolute inset-0 flex items-center justify-center">
            <!-- Overlay text if needed -->
        </div>
      </div>
      <div class="aspect-[3/4] bg-gray-200 overflow-hidden group">
        <img src={labImage} alt="Engineering team collaboration" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
      </div>
    </div>
  </section>

  <!-- Partners Section -->
  <section class="py-24 px-6 max-w-[1400px] mx-auto">
    <h2 class="text-3xl md:text-4xl font-normal mb-16">Government & Industry Partners</h2>
    
    <!-- Government -->
    <div class="mb-20 border-t border-gray-200 pt-8">
      <div class="mb-8">
        <h3 class="text-lg font-normal mb-2">Government Support</h3>
        <p class="text-[11px] text-gray-500 max-w-md leading-tight">$11M from Government of Canada through Natural Resources Canada to advance Small Modular Reactor Research and Hydrogen Technologies</p>
      </div>
      <div class="flex flex-wrap items-center gap-12 md:gap-24 grayscale opacity-100">
        {#each partnersGov as partner}
           <img src={partner.src} alt={partner.name} class="h-14 w-auto object-contain mix-blend-multiply" />
        {/each}
      </div>
    </div>

    <!-- Industry -->
    <div class="border-t border-gray-200 pt-8">
      <div class="mb-8">
        <h3 class="text-lg font-normal mb-2">Industry Focus</h3>
        <p class="text-[11px] text-gray-500 max-w-md leading-tight">Serving operations managers at oil sands, mining, and petrochemical facilities who need equipment uptime but face costly wear failures</p>
      </div>
      <div class="flex flex-wrap items-center gap-8 md:gap-12">
        {#each partnersIndustry as partner}
           <div class="px-6 py-3 border border-gray-300 text-sm text-gray-700 font-medium">
             {partner.name}
           </div>
        {/each}
      </div>
    </div>
  </section>

  <!-- Join Us Section -->
  <section class="py-24 px-6 max-w-[1400px] mx-auto">
    <h2 class="text-4xl md:text-5xl font-normal mb-16">Join Us</h2>
    
    <div class="space-y-0">
      {#each jobs as job, i}
        {#if i === 0 || jobs[i-1].category !== job.category}
           <div class="pt-8 pb-4 border-b border-gray-200 mt-8 first:mt-0">
             <h3 class="text-xl font-normal">{job.category}</h3>
           </div>
        {/if}
        <div class="py-4 border-b border-gray-200 flex flex-col md:flex-row justify-between md:items-center gap-2 group cursor-pointer hover:bg-gray-50 transition-colors px-2 -mx-2">
          <span class="text-sm font-medium text-gray-800">{job.title}</span>
          <span class="text-[11px] text-gray-500">{job.location}</span>
        </div>
      {/each}
    </div>
  </section>

  <!-- CTA Banner -->
  <section class="px-6 pb-24 max-w-[1400px] mx-auto">
    <div class="bg-[#222] text-white p-12 md:p-16 flex flex-col md:flex-row items-center justify-between gap-8 rounded-sm">
      <h2 class="text-3xl md:text-4xl font-normal max-w-md leading-tight">
        Partner with Quantiam for extreme wear protection solutions
      </h2>
      <button class="bg-white/20 hover:bg-white/30 backdrop-blur-sm text-white px-6 py-2 rounded-full text-[11px] font-bold uppercase tracking-widest flex items-center gap-2 transition-colors">
        Contact Us <span class="text-xs">→</span>
      </button>
    </div>
  </section>

  <Footer />
</main>


