<script>
	let arr = []
	let obj = {name: 'ashnamuh'}

	const handleClick = () => {
		// arr = [...arr, 'item']
		arr.push('item') // Not working

		obj = {...obj, age: 23 }
		// obj.age = 23 Also not working
	}

	const handleClick2 = () => {
		arr = [...arr, 'item']
		// arr.push('item') // Not working

		obj = {...obj, age: 23 }
		// obj.age = 23 Also not working
	}
</script>

<button on:click={handleClick}>
	click me to add item
</button>
<button on:click={handleClick2}>
	show me
</button>
<p>{arr.join(' ')}</p>
<p>{Object.values(obj)}</p>