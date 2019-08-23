<script>
import { onMount } from 'svelte'
import Cat from './Cat.svelte'
import Dog from './Dog.svelte'

const options = [
  { animal: 'cat', component: Cat },
  { animal: 'dog', component: Dog }
]

let selected = options[0]
let b
onMount(() => {
  console.log(b)
  console.log('b')
})
const handleClick = () => console.log('clicked!')
</script>

<svelte:body bind:this={b} on:click={handleClick} />
<svelte:head>
  <title>ashnamuh 개발 블로그</title>
  <meta name="description" content="ashnamuh의 개발 블로그입니다.">
</svelte:head>

<select bind:value={selected}>
  <option value={options[0]}>고양이</option>
  <option value={options[1]}>개</option>
</select>

<svelte:component this={selected.component}/>