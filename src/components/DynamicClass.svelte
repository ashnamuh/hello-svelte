<script>
let toggled = false

const toggle = () => toggled = !toggled
</script>

<style>
.toggled {
  background-color: #ffff00;
}
</style>

<button on:click={toggle}>toggle</button>
<p class:toggled={toggled === true}>yellow, if toggled</p>