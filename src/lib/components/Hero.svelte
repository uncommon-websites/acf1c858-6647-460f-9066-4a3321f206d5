<script>
  let activeTab = 'Public Equities';
  const tabs = ['Public Equities', 'Fixed Income', 'Private Equity', 'Real Estate', 'Infrastructure', 'Credit', 'Alternatives', 'Cash & Liquidity'];
</script>

<section class="pt-32 pb-20 px-6 max-w-7xl mx-auto">
  <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 mb-16">
    <div>
      <h1 class="text-5xl md:text-6xl font-medium tracking-tight text-black leading-[1.1] mb-8">
        Sustaining prosperity <br /> through global investment
      </h1>
    </div>
    <div class="flex flex-col justify-end items-start lg:pl-12">
      <p class="text-xl text-gray-600 mb-6 max-w-md leading-relaxed">
        A globally diversified investment institution managing Abu Dhabi's wealth with a long-term perspective across all major asset classes.
      </p>
      <a href="#" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
        Explore Opportunities 
        <span class="ml-1 group-hover:translate-x-1 transition-transform">→</span>
      </a>
    </div>
  </div>

  <!-- Interactive Visual Section -->
  <div class="rounded-3xl overflow-hidden bg-gray-50 border border-gray-200 shadow-sm">
    <!-- Tabs -->
    <div class="flex overflow-x-auto scrollbar-hide border-b border-gray-200 bg-white/50 backdrop-blur-sm">
      {#each tabs as tab}
        <button 
          class="px-5 py-4 text-sm font-medium whitespace-nowrap transition-colors relative {activeTab === tab ? 'text-black' : 'text-gray-500 hover:text-gray-800'}"
          on:click={() => activeTab = tab}
        >
          {tab}
          {#if activeTab === tab}
            <div class="absolute bottom-0 left-0 right-0 h-0.5 bg-black"></div>
          {/if}
        </button>
      {/each}
    </div>

    <!-- Content Area -->
    <div class="relative h-[500px] bg-gradient-to-br from-gray-900 to-gray-800 overflow-hidden group">
      <!-- Background Image Placeholder -->
      <img 
        src="https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?q=80&w=2560&auto=format&fit=crop" 
        alt="Global financial markets" 
        class="absolute inset-0 w-full h-full object-cover opacity-30 transition-transform duration-700 group-hover:scale-105"
      />
      
      <!-- Floating Portfolio Card -->
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-96 bg-white/10 backdrop-blur-md border border-white/20 rounded-2xl p-6 text-white shadow-2xl">
        <div class="flex justify-between items-center mb-6">
          <span class="text-xs font-medium text-white/80">Global Portfolio Overview</span>
          <span class="text-xs text-white/60">Since 1976</span>
        </div>
        
        <!-- Asset Allocation -->
        <div class="space-y-4">
          <div class="flex items-center gap-3">
            <div class="w-10 h-10 rounded-lg bg-blue-500/80 flex items-center justify-center text-white shrink-0">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M3 13h8V3H3v10zm0 8h8v-6H3v6zm10 0h8V11h-8v10zm0-18v6h8V3h-8z"/></svg>
            </div>
            <div class="flex-1 min-w-0">
              <div class="flex justify-between items-baseline">
                <h3 class="text-sm font-medium">Public Equities</h3>
                <span class="text-sm font-medium">32%</span>
              </div>
              <p class="text-xs text-white/60">Developed & Emerging Markets</p>
            </div>
          </div>

          <div class="flex items-center gap-3">
            <div class="w-10 h-10 rounded-lg bg-teal-500/80 flex items-center justify-center text-white shrink-0">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zM9 17H7v-7h2v7zm4 0h-2V7h2v10zm4 0h-2v-4h2v4z"/></svg>
            </div>
            <div class="flex-1 min-w-0">
              <div class="flex justify-between items-baseline">
                <h3 class="text-sm font-medium">Fixed Income</h3>
                <span class="text-sm font-medium">20%</span>
              </div>
              <p class="text-xs text-white/60">Government & Corporate Bonds</p>
            </div>
          </div>

          <div class="flex items-center gap-3">
            <div class="w-10 h-10 rounded-lg bg-purple-500/80 flex items-center justify-center text-white shrink-0">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"/></svg>
            </div>
            <div class="flex-1 min-w-0">
              <div class="flex justify-between items-baseline">
                <h3 class="text-sm font-medium">Alternatives</h3>
                <span class="text-sm font-medium">48%</span>
              </div>
              <p class="text-xs text-white/60">PE, RE, Infrastructure & Credit</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Key Metrics -->
    <div class="bg-gray-50 p-8 border-t border-gray-200">
      <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
        <div>
          <div class="text-3xl font-bold text-black mb-1">65+</div>
          <div class="text-sm text-gray-600">Nationalities</div>
        </div>
        <div>
          <div class="text-3xl font-bold text-black mb-1">54</div>
          <div class="text-sm text-gray-600">Languages Spoken</div>
        </div>
        <div>
          <div class="text-3xl font-bold text-black mb-1">180+</div>
          <div class="text-sm text-gray-600">CFA Charterholders</div>
        </div>
        <div>
          <div class="text-3xl font-bold text-black mb-1">1976</div>
          <div class="text-sm text-gray-600">Founded</div>
        </div>
      </div>
    </div>
  </div>
</section>
