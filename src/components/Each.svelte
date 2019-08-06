<script>
let people = [
  { id: 1, name: 'ashnamuh' },
  { id: 2, name: 'Jaemok Lee' },
  { id: 3, name: 'Ash Lee' }
]
</script>

<ul>
  {#each people as person, index}
    <li>
      index: {index}
      id: {person.id}
      name: {person.name}
    </li>
  {/each}
</ul>