<script>
let count = 0;

$: doubled = count * 2;

setInterval(() => {
	count++
}, 1000)
</script>

<p>count: {count}</p>
<p>doubled: {doubled}</p>