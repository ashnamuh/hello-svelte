<script>
  let user = { loggedIn: false }

  const toggle = () => {
    user.loggedIn = !user.loggedIn
  }
  let count = 10
</script>

{#if user.loggedIn}
  <button on:click={toggle}>
    Log out
  </button>
{/if}

{#if !user.loggedIn}
  <button on:click={toggle}>
    Log in
  </button>
{/if}

{#if count > 10}
  <p>{count}는 10 초과</p>
{:else if 5 > count}
  <p>{count}는 5 미만</p>
{:else}
  <p>{count}는 5이상 10 이하</p>
{/if}