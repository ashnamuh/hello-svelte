<script>
import TheHeader from './components/TheHeader.svelte';
import Count from './components/Count.svelte';
import Event from './components/Event.svelte';

const name = 'ashnamuh';

</script>

<style>
	h1 {
		color: blue;
	}
</style>

<TheHeader></TheHeader>
<h1>Hello {name}!</h1>
<Count></Count>
<Event></Event>