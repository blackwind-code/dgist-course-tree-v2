<script>
  /**
   * @type {string}
   */
  export let name;
  import IoIosAdd from "svelte-icons/io/IoIosAdd.svelte";
</script>

<div class="p-2 rounded-sm hover:bg-slate-600 flex flex-row items-center select-none cursor-copy">
  <div class="flex-1">{name}</div>
  <div class="w-6 h-6">
    <IoIosAdd></IoIosAdd>
  </div>
</div>
