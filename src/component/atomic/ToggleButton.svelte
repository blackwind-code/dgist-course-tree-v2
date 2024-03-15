<script>
  /**
   * @type {boolean}
   */
  export let selected;
  /**
   * @type {string}
   */
   export let name;
</script>

<div
  class="{selected
    ? 'bg-white text-bg border-bw border-2'
    : 'bg-bw text-white'} max-w-36 rounded-md p-2 flex flex-row items-center select-none min-h-10"
>
  {name}
</div>
