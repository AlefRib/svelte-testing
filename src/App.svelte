<script lang="ts">
  import logo from './assets/svelte.png'
  import menu from './assets/hamburguer-menu.svg'
  import Counter from './lib/Counter.svelte'
</script>

<main class="text-center mx-0">
  <div class="bg-indigo-600 text-cyan-500 p-5 flex items-center justify-between" >
    <div>
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24 w-5" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
        <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
      </svg>
    </div>
    <img class="w-10" alt="logo" src={logo}/>
    <div>
      <button class="max-w-xs sm:max-w-none my-4 text-lg font-semibold bg-cyan-500 text-indigo-600 p-3 rounded-full mr-4">
        Quer Ajudar?
      </button>
      <button  class="max-w-xs sm:max-w-none my-4 text-lg font-semibold  ">
       Entre em contato
      </button>
    </div>
  </div>
</main>

<style lang="postcss">
  :root {
    --svelte-rgb: 255, 62, 0;
    background-color: rgb(79 70 229);
  }

  h1 {
    color: rgb(var(--svelte-rgb));
  }
</style>