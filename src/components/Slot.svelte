<script>
import { onMount } from 'svelte'
import Link from './Link.svelte'
import Page from './Page.svelte'

let element

onMount(() => {
  console.log(element)
})
</script>

<div id="container">container element</div>
<Link>Link to Svelte!<i class="link" /></Link>
<Page let:username={pageUsername} bind:this={element}>
  <header slot="header">{pageUsername}의 소개 페이지!</header>
  <footer slot="footer">주입하는 푸터</footer>
</Page>