<script>
  export let count = 5
</script>

{#if count > 0}
  <p>카운트가 내려갑니다 {count}</p>
  <svelte:self count="{count - 1}"/>
{:else}
  <p>카운트가 {count}되었습니다!</p>
{/if}