<script lang="ts">
  import { invoke } from "@tauri-apps/api/tauri"

  let name = "";
  let greetMsg = ""

  async function greet(){
    // Learn more about Tauri commands at https://tauri.app/v1/guides/features/command
    greetMsg = await invoke("greet", { name })
  }
</script>

<div>
  <form class="flex flex-col" on:submit|preventDefault={greet}>
    <input class="bg-slate-900 p-2 rounded-lg" id="greet-input" placeholder="Enter a name..." bind:value={name} />
    <button class="bg-slate-500 p-2 rounded-lg font-semibold" type="submit">Greet</button>
  </form>
  <p class="text-center font-semibold">{greetMsg}</p>
</div>