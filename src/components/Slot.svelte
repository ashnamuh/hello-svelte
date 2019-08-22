<script>
import Link from './Link.svelte'
import Page from './Page.svelte'

</script>

<Link>Link to Svelte!<i class="link" /></Link>
<Page>
  <header slot="header">주입하는 헤더</header>
  <footer slot="footer">주입하는 푸터</footer>
</Page>