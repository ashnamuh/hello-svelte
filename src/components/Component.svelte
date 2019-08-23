<script>
  import Cat from './Cat.svelte'
  import Dog from './Dog.svelte'

  const options = [
    { animal: 'cat', component: Cat },
    { animal: 'dog', component: Dog }
  ]

  let selected = options[0]
</script>

<select bind:value={selected}>
  <option value={options[0]}>고양이</option>
  <option value={options[1]}>개</option>
</select>

<svelte:component this={selected.component}/>