<script>
let count = 0;

$: doubled = count * 2;

$: console.log(`the count is ${count}`);

setInterval(() => {
	count++
}, 1000)
</script>

<p>count: {count}</p>
<p>doubled: {doubled}</p>