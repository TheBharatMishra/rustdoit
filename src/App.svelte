<script lang="ts">
  import Greet from './lib/Greet.svelte'
</script>

<main class="flex flex-col justify-start items-center bg-slate-800 h-screen">
  <h1 class="text-5xl font-bold bg-slate-600 w-full text-center text-slate-800 p-4 m-4">RUST DO IT</h1>

  <a class="size-48" href="https://parallelintersect.vercel.app" target="_blank">
    <img src="/logo.svg" class="logo tauri" alt="Tauri Logo" />
  </a>
  <div class="size-96">
  <p class="text-center font-semibold">we make impossible, possible.</p>

  <div class="">
    <Greet />
  </div>


</main>

