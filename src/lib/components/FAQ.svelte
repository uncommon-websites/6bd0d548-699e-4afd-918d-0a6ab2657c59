<script lang="ts">
  import { slide } from 'svelte/transition';
  
  interface FAQItem {
    question: string;
    answer: string;
  }

  const faqs: FAQItem[] = [
    { question: "How is Tatem different from Gmail or Outlook?", answer: "Tatem is built from the ground up for speed and focus. We offer sub-50ms response times, intelligent inbox splitting to separate important emails from clutter, and a keyboard-first design that keeps you in flow. Unlike traditional email clients, we prioritize delight and craft in every interaction." },
    { question: "How fast is Tatem really?", answer: "Every interaction in Tatem happens in under 50 milliseconds. That's faster than you can blink. We've eliminated the lag and delays that make traditional email feel sluggish, so you can process your inbox at the speed of thought." },
    { question: "Does Tatem work with my existing email?", answer: "Yes! Tatem works with your existing Gmail, Outlook, or other email accounts. We don't store your emails or passwords—everything stays secure and private while you get a dramatically better experience." },
    { question: "What about privacy and security?", answer: "Privacy is core to how we built Tatem. We store zero emails in our database, zero passwords, and zero payment information. Your data stays yours, always. We use enterprise-grade security with a privacy-first architecture." },
    { question: "Is Tatem available now?", answer: "Tatem is currently in early access with 10,000+ users. We're onboarding new users gradually to ensure everyone gets the best experience. Sign up to join the waitlist and we'll get you in as soon as possible." },
    { question: "How much does Tatem cost?", answer: "We're currently focused on building the best email experience possible. Pricing details will be shared as we move closer to general availability. Early access users will get special consideration." },
    { question: "Can I use Tatem on mobile?", answer: "Yes! Tatem works across desktop and mobile. Our mobile engineer is ensuring the same speed and delight translates perfectly to your phone." }
  ];

  let openIndex: number | null = null;

  function toggle(index: number) {
    openIndex = openIndex === index ? null : index;
  }
</script>

<section class="bg-[#f5f5f5] px-6 py-24">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-4">
      <h2 class="font-serif text-4xl text-gray-900 mb-6">
        Frequently asked questions
      </h2>
      <a href="/" class="text-sm text-gray-900 border-b border-gray-300 pb-0.5 hover:border-black transition-colors">See all support</a>
    </div>
    
    <div class="lg:col-span-8">
      <div class="border-t border-gray-200">
        {#each faqs as faq, i}
          <div class="border-b border-gray-200">
            <button 
              class="w-full py-6 flex justify-between items-center text-left hover:bg-gray-50 transition-colors"
              on:click={() => toggle(i)}
            >
              <span class="text-lg text-gray-800">{faq.question}</span>
              <span class="text-2xl font-light text-gray-400 ml-4">
                {openIndex === i ? '−' : '+'}
              </span>
            </button>
            {#if openIndex === i}
              <div transition:slide class="pb-6 text-gray-500 leading-relaxed">
                {faq.answer}
              </div>
            {/if}
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>
