<script>
  // No script needed
</script>

<div class="space-y-32 pb-32">
  <!-- Public Markets Section -->
  <section class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
    <div>
      <h3 class="text-4xl font-medium mb-6">Public Markets</h3>
      <p class="text-xl text-gray-600 mb-8 leading-relaxed">
        <strong class="text-black">Global equity and fixed income expertise.</strong> Managing diversified portfolios across developed and emerging markets with deep fundamental research and quantitative capabilities.
      </p>
      <div class="flex flex-col gap-2">
        <a href="#" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
          Explore opportunities 
          <span class="ml-1 group-hover:translate-x-1 transition-transform">→</span>
        </a>
        <a href="#" class="text-sm text-gray-400 hover:text-black transition-colors">View open positions</a>
      </div>
    </div>
    <div class="bg-gray-50 rounded-3xl p-12 flex items-center justify-center min-h-[400px]">
      <!-- Global Markets Visualization -->
      <div class="relative w-full max-w-md">
        <div class="grid grid-cols-3 gap-4">
          {#each [
            { name: 'Americas', value: '35%', color: 'bg-blue-500' },
            { name: 'Europe', value: '28%', color: 'bg-teal-500' },
            { name: 'Asia Pacific', value: '20%', color: 'bg-purple-500' },
            { name: 'Equities', value: '60%', color: 'bg-indigo-500' },
            { name: 'Fixed Income', value: '40%', color: 'bg-cyan-500' },
            { name: 'Global', value: '100%', color: 'bg-black' }
          ] as region}
            <div class="text-center">
              <div class="w-16 h-16 {region.color} rounded-lg mx-auto mb-2 flex items-center justify-center text-white font-bold text-sm">
                {region.value}
              </div>
              <div class="text-xs text-gray-600 font-medium">{region.name}</div>
            </div>
          {/each}
        </div>
      </div>
    </div>
  </section>

  <!-- Private Markets Section -->
  <section class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
    <div>
      <h3 class="text-4xl font-medium mb-6">Private Markets</h3>
      <p class="text-xl text-gray-600 mb-8 leading-relaxed">
        <strong class="text-black">Long-term value creation.</strong> Investing in private equity, real estate, infrastructure, and credit with patient capital and deep sector expertise across global markets.
      </p>
      <div class="flex flex-col gap-2">
        <a href="#" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
          Explore opportunities 
          <span class="ml-1 group-hover:translate-x-1 transition-transform">→</span>
        </a>
        <a href="#" class="text-sm text-gray-400 hover:text-black transition-colors">View open positions</a>
      </div>
    </div>
    <div class="bg-gradient-to-br from-gray-50 to-gray-100 rounded-3xl overflow-hidden min-h-[400px] relative p-8">
      <div class="space-y-4">
        {#each [
          { label: 'Private Equity', icon: '🏢' },
          { label: 'Real Estate', icon: '🏗️' },
          { label: 'Infrastructure', icon: '🌉' },
          { label: 'Credit', icon: '💼' }
        ] as asset}
          <div class="bg-white/80 backdrop-blur-sm rounded-xl p-4 flex items-center gap-4 shadow-sm hover:shadow-md transition-shadow">
            <div class="text-2xl">{asset.icon}</div>
            <div class="text-base font-medium text-gray-800">{asset.label}</div>
          </div>
        {/each}
      </div>
    </div>
  </section>

  <!-- Innovation & Research Section -->
  <section class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
    <div>
      <h3 class="text-4xl font-medium mb-6">Innovation & Research</h3>
      <p class="text-xl text-gray-600 mb-8 leading-relaxed">
        <strong class="text-black">Pioneering investment approaches.</strong> Leading research in quantitative methods, climate integration, and emerging technologies. Home to Quants of the Year and industry-shaping frameworks.
      </p>
      <div class="flex flex-col gap-2">
        <a href="#" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
          Explore opportunities 
          <span class="ml-1 group-hover:translate-x-1 transition-transform">→</span>
        </a>
        <a href="#" class="text-sm text-gray-400 hover:text-black transition-colors">View open positions</a>
      </div>
    </div>
    <div class="bg-gradient-to-br from-gray-900 to-black rounded-3xl p-12 flex items-center justify-center min-h-[400px]">
      <!-- Research Highlights -->
      <div class="space-y-6 text-white w-full">
        <div class="border-l-4 border-teal-500 pl-4">
          <div class="text-sm text-gray-400 mb-1">Recognition</div>
          <div class="text-base font-medium">Quants of the Year 2021</div>
          <div class="text-xs text-gray-500">Risk Awards</div>
        </div>
        <div class="border-l-4 border-blue-500 pl-4">
          <div class="text-sm text-gray-400 mb-1">Leadership</div>
          <div class="text-base font-medium">Santiago Principles Co-Chair</div>
          <div class="text-xs text-gray-500">IMF Partnership 2008</div>
        </div>
        <div class="border-l-4 border-purple-500 pl-4">
          <div class="text-sm text-gray-400 mb-1">Sustainability</div>
          <div class="text-base font-medium">One Planet SWF Framework</div>
          <div class="text-xs text-gray-500">Climate Integration 2018</div>
        </div>
        <div class="border-l-4 border-green-500 pl-4">
          <div class="text-sm text-gray-400 mb-1">Innovation</div>
          <div class="text-base font-medium">Early PE & Hedge Fund Adoption</div>
          <div class="text-xs text-gray-500">Pioneering 1980s</div>
        </div>
      </div>
    </div>
  </section>
</div>
