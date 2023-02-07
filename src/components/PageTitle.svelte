<script>
  export let title = "";
  export let subtitle = "";
</script>

<div class="h-64 flex justify-center items-center relative">
  <h1
    class=" z-0 text-9xl text-opacity-10 text-white mb-8 font-semibold absolute"
  >
    {subtitle}
  </h1>
  <h1 class=" z-10 text-5xl text-white font-semibold">{title}</h1>
</div>
