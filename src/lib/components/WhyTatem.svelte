<script>
  import SectionLabel from './SectionLabel.svelte';
</script>

<section class="bg-[#f5f5f5] px-6 py-24">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-3">
      <SectionLabel label="Why Tatem" />
    </div>
    
    <div class="lg:col-span-9 grid grid-cols-1 md:grid-cols-2 gap-16">
      <div>
        <h2 class="font-serif text-3xl md:text-4xl leading-tight text-gray-900 mb-6">
          Email hasn't meaningfully evolved in decades. We're changing that.
        </h2>
        <p class="text-gray-500 leading-relaxed">
          Built by misfits, artists, and pirates who believe software should spark joy. We're bringing delight to a product used by billions.
        </p>
      </div>
      
      <div class="flex gap-12 items-end pb-2">
        <div class="flex flex-col gap-1">
            <span class="text-4xl font-serif text-gray-900 mb-1">&lt;50ms</span>
            <span class="text-xs text-gray-400">response time</span>
        </div>
        <div class="flex flex-col gap-1">
            <span class="text-4xl font-serif text-gray-900 mb-1">10,000+</span>
            <span class="text-xs text-gray-400">early users</span>
        </div>
      </div>
    </div>
  </div>
</section>
