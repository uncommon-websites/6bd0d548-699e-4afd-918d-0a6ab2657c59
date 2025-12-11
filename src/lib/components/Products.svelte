<script>
  import SectionLabel from './SectionLabel.svelte';
</script>

<section class="bg-[#f5f5f5] px-6 py-24 border-t border-gray-200">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-3">
      <SectionLabel label="Features" />
    </div>
    
    <div class="lg:col-span-9">
      <div class="mb-16">
        <h2 class="font-serif text-4xl md:text-5xl text-gray-900 mb-2">
          Simplicity, speed,
        </h2>
        <h2 class="font-serif text-4xl md:text-5xl text-gray-400">
          and intelligence
        </h2>
      </div>

      <div class="grid gap-0 border-t border-gray-200">
        <!-- Item 1 -->
        <div class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-gray-200 hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">Core feature</div>
            <h3 class="text-2xl font-medium text-gray-900">Intelligent inbox splitting</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-500 leading-relaxed">
              Automatically separates important emails from spam and marketing clutter. Focus on what matters while everything else stays organized but out of sight.
            </p>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-black transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </div>

        <!-- Item 2 -->
        <div class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-gray-200 hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">Performance</div>
            <h3 class="text-2xl font-medium text-gray-900">Sub-50ms interactions</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-500 leading-relaxed">
              Every action feels instant. No lag, no waiting, no frustration. We've eliminated the delays that break your flow and make email feel like a chore.
            </p>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-black transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </div>

        <!-- Item 3 -->
        <div class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-gray-200 hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">Design</div>
            <h3 class="text-2xl font-medium text-gray-900">Keyboard-first experience</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-500 leading-relaxed">
              Familiar shortcuts you already know. Navigate, compose, and manage email without touching your mouse. Elegant transitions and a modern text editor make every interaction delightful.
            </p>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-black transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </div>

        <!-- Item 4 -->
        <div class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-gray-200 hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">Privacy & Security</div>
            <h3 class="text-2xl font-medium text-gray-900">Enterprise-grade security</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-500 leading-relaxed">
              Zero email storage in our database. Zero password storage. Zero payment information. Privacy-first architecture means your data stays yours.
            </p>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-black transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
