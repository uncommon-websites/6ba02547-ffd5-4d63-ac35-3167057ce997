<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Footer from "$lib/components/Footer.svelte";
  
  // Images
  const heroImage = "https://images.unsplash.com/photo-1542296332-2e44a996aa0b?q=80&w=2574&auto=format&fit=crop";
  const factoryImage = "https://images.unsplash.com/photo-1565610222536-ef125c59da2e?q=80&w=2670&auto=format&fit=crop";
  const presentationImage = "https://images.unsplash.com/photo-1544531586-fde5298cdd40?q=80&w=2670&auto=format&fit=crop";
  const labImage = "https://images.unsplash.com/photo-1581093458791-9f3c3900df4b?q=80&w=2670&auto=format&fit=crop";

  // Logos (Using text/SVGs for now as placeholders)
  const partnersGov = [
    { name: "U.S. Department of Defense", src: "https://upload.wikimedia.org/wikipedia/commons/e/e0/United_States_Department_of_Defense_Seal.svg" },
    { name: "U.S. Department of State", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/8/81/U.S._Department_of_State_official_seal.svg/2048px-U.S._Department_of_State_official_seal.svg.png" },
    { name: "Defense Innovation Unit", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/e/e4/Defense_Innovation_Unit_logo.jpg/800px-Defense_Innovation_Unit_logo.jpg" },
    { name: "NASA", src: "https://upload.wikimedia.org/wikipedia/commons/e/e5/NASA_logo.svg" },
    { name: "U.S. Air Force", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/d/d1/Mark_of_the_United_States_Air_Force.svg/2448px-Mark_of_the_United_States_Air_Force.svg.png" },
  ];

  const partnersAviation = [
    { name: "Air Canada", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/2/22/Air_Canada_Logo.svg/2560px-Air_Canada_Logo.svg.png" },
    { name: "JetBlue", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/3/3b/JetBlue_Airways_Logo.svg/2560px-JetBlue_Airways_Logo.svg.png" },
    { name: "Virgin Atlantic", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/0/01/Virgin_Atlantic_logo.svg/2560px-Virgin_Atlantic_logo.svg.png" },
    { name: "Air France KLM", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/4/44/Air_France-KLM_Logo.svg/2560px-Air_France-KLM_Logo.svg.png" },
    { name: "Alaska Airlines", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/66/Alaska_Airlines_logo.svg/2560px-Alaska_Airlines_logo.svg.png" },
    { name: "Avfuel", src: "https://upload.wikimedia.org/wikipedia/en/thumb/3/36/Avfuel_Corporation_Logo.svg/1200px-Avfuel_Corporation_Logo.svg.png" },
  ];

  const jobs = [
    { category: "Future Opportunities", title: "Don't see the job you're looking for? Reach out anyway", location: "Brooklyn, New York, United States" },
    { category: "Government & Defense", title: "Senior Manager, DoD Acquisition", location: "New Britain, Pennsylvania, United States" },
    { category: "Operations", title: "Process Operator III (New Britain, PA)", location: "New Britain, Pennsylvania, United States" },
    { category: "Operations", title: "Procurement & Accounts Payable Specialist", location: "New Britain, Pennsylvania, United States" },
    { category: "Operations", title: "Strategic Sourcing Manager, Fuel Production Systems", location: "New Britain, Pennsylvania, United States" },
    { category: "Operations", title: "Process Engineer", location: "New Britain, Pennsylvania, United States" },
    { category: "RD&E", title: "Director, Engineering", location: "New Britain, Pennsylvania, United States" },
  ];
</script>

<Header />

<main class="font-sans text-black selection:bg-gray-200 pt-16">
  <!-- Hero Section -->
  <section class="relative h-[85vh] w-full overflow-hidden">
    <div class="absolute inset-0 bg-black/20 z-10"></div>
    <img 
      src={heroImage} 
      alt="Turbine engine" 
      class="w-full h-full object-cover object-center"
    />
    <div class="absolute inset-0 z-20 flex items-center justify-center">
      <h1 class="text-white text-5xl md:text-7xl font-normal text-center leading-tight max-w-4xl mx-auto px-4 drop-shadow-lg">
        Leaders in Synthetic<br />Fuel Technology
      </h1>
    </div>
  </section>

  <!-- Intro Section -->
  <section class="py-24 px-6 max-w-[1400px] mx-auto">
    <div class="grid grid-cols-1 md:grid-cols-12 gap-12">
      <div class="md:col-span-4">
        <h2 class="text-2xl font-normal tracking-wide mb-2 uppercase">AIR COMPANY</h2>
        <p class="text-[10px] font-bold tracking-widest uppercase text-gray-500">AIRMADE™</p>
      </div>
      <div class="md:col-span-8 grid grid-cols-1 md:grid-cols-2 gap-12 relative">
        <div class="col-span-2 md:col-span-2 space-y-6 text-[15px] leading-relaxed text-gray-800 max-w-3xl font-light">
          <p>
            AIRCO is a global leader in carbon conversion technology. We are committed to achieving global energy independence and security by transforming carbon dioxide (CO₂) into fully-formulated synthetic fuels.
          </p>
          <p>
            Our proprietary AIRMADE™ Technology is a versatile platform that enables industries to produce fuels locally while reducing greenhouse gas emissions. This is achieved by producing high-demand, fully-formulated synthetic fuels from CO₂ and hydrogen (H₂). Currently focused on fuel applications, AIRCO's goal is to deploy the most cost-effective and scalable fuel production technology on the market.
          </p>
          <p>
            AIRCO is a carbon utilization technology provider offering licensing packages for its proprietary AIRMADE™ products such as sustainable aviation fuel (SAF), methanol, ethanol, paraffins, and aromatics through advanced catalytic carbon conversion.
          </p>
          <p>
            AIRCO is an industry leader in AIRMADE™ Ethanol research, manufacturing, processing, and development, providing technical consultation and research assistance to others in ethanol production and processing.
          </p>
        </div>
        
        <!-- Logo Mark -->
        <div class="absolute -bottom-12 right-0 hidden md:block">
           <svg viewBox="0 0 24 24" class="w-12 h-12" fill="currentColor">
            <path d="M12 2.5C13.5 8.5 18 11.5 22.5 12C18 12.5 13.5 15.5 12 21.5C10.5 15.5 6 12.5 1.5 12C6 11.5 10.5 8.5 12 2.5Z" />
          </svg>
        </div>
      </div>
    </div>
  </section>

  <!-- Factory Image -->
  <section class="w-full px-6 pb-24 max-w-[1400px] mx-auto">
    <div class="aspect-[16/9] w-full overflow-hidden bg-gray-100">
      <img src={factoryImage} alt="Factory interior" class="w-full h-full object-cover" />
    </div>
  </section>

  <!-- Team Section -->
  <section class="py-24 px-6 max-w-[1400px] mx-auto border-t border-transparent">
    <div class="grid grid-cols-1 md:grid-cols-12 gap-12">
      <div class="md:col-span-4">
        <h2 class="text-4xl md:text-5xl font-normal tracking-tight">The AIRCO Team</h2>
      </div>
      <div class="md:col-span-8 space-y-8">
        <p class="text-[15px] leading-relaxed text-gray-800 font-light max-w-3xl">
          Founded in 2017 by Gregory Constantine and Dr. Stafford Sheehan, the AIRCO team has a core foundation in energy, tech, and defense. Our dynamic team of industry veterans brings deep expertise across all business areas. From R&D and engineering to operations, logistics, and policy, we leverage years of experience to develop scalable fuel innovation solutions.
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
        <img src={presentationImage} alt="Presentation" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
        <div class="absolute inset-0 flex items-center justify-center">
            <!-- Overlay text if needed -->
        </div>
      </div>
      <div class="aspect-[3/4] bg-gray-200 overflow-hidden group">
        <img src={labImage} alt="Lab worker" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
      </div>
    </div>
  </section>

  <!-- Partners Section -->
  <section class="py-24 px-6 max-w-[1400px] mx-auto">
    <h2 class="text-3xl md:text-4xl font-normal mb-16">Government & Aviation Partners</h2>
    
    <!-- Government -->
    <div class="mb-20 border-t border-gray-200 pt-8">
      <div class="mb-8">
        <h3 class="text-lg font-normal mb-2">Government</h3>
        <p class="text-[11px] text-gray-500 max-w-xs leading-tight">U.S. government support helps to drive R&D and future commercial opportunities</p>
      </div>
      <div class="flex flex-wrap items-center gap-12 md:gap-24 grayscale opacity-100">
        {#each partnersGov as partner}
           <img src={partner.src} alt={partner.name} class="h-14 w-auto object-contain mix-blend-multiply" />
        {/each}
      </div>
    </div>

    <!-- Aviation -->
    <div class="border-t border-gray-200 pt-8">
      <div class="mb-8">
        <h3 class="text-lg font-normal mb-2">Aviation</h3>
        <p class="text-[11px] text-gray-500 max-w-xs leading-tight">AIRMADE® SAF customers and corporate funding backers</p>
      </div>
      <div class="flex flex-wrap items-center gap-12 md:gap-24 grayscale opacity-100">
        {#each partnersAviation as partner}
           <img src={partner.src} alt={partner.name} class="h-8 md:h-10 w-auto object-contain mix-blend-multiply" />
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
        Learn how you can partner with AIRCO
      </h2>
      <button class="bg-white/20 hover:bg-white/30 backdrop-blur-sm text-white px-6 py-2 rounded-full text-[11px] font-bold uppercase tracking-widest flex items-center gap-2 transition-colors">
        Contact Us <span class="text-xs">→</span>
      </button>
    </div>
  </section>

  <Footer />
</main>


