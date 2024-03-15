<script lang="ts">
  import svelteLogo from "./assets/svelte.svg";
  import viteLogo from "/vite.svg";
  import Counter from "./lib/Counter.svelte";
  import Lecture from "./component/atomic/Lecture.svelte";
  import ToggleButton from "./component/atomic/ToggleButton.svelte";
</script>

<main class="flex">
  <div class="w-80 bg-slate-900 h-screen overflow-scroll text-slate-200">
    <div class="flex flex-col gap-2 py-4 sticky top-0 bg-slate-900">
      <button class="border rounded-sm py-2 mx-4">reset</button>
      <button class="border rounded-sm py-2 mx-4">save</button>
    </div>
    <div class="flex flex-1 flex-col" id="leftside">
      <div class="px-4">
        <div class="text-lg font-bold pb-2">Essential</div>
        <div class="flex flex-col gap-2">
          <Lecture name={"Biology"}></Lecture>
        </div>
      </div>
    </div>
  </div>
  <div class="flex flex-col gap-4 flex-1 bg-slate-100">
    <div>Choose your Major</div>
    <div class="grid grid-rows-2 gap-2">
      <ToggleButton name="Computer" selected></ToggleButton>
      <ToggleButton name="Computer" selected={false}></ToggleButton>
    </div>
    <div class="flex text-sm gap-4">
      <div class="flex items-center gap-3 p-2 rounded border bg-white shadow">
        <div class="w-4 h-4 bg-red-600 rounded-full"></div>
        <div>Essential 3/24</div>
      </div>
      <div class="flex items-center gap-3 p-2 rounded border">
        <div class="w-4 h-4 bg-red-600 rounded-full"></div>
        <div>Essential 3/24</div>
      </div>
    </div>
  </div>
</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
  .read-the-docs {
    color: #888;
  }
</style>
