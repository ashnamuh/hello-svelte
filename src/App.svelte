<script>
import TheHeader from './components/TheHeader.svelte'
import Count from './components/Count.svelte'
import Event from './components/Event.svelte'
import Props from './components/Props.svelte'
import ArrayList from './components/ArrayList.svelte'
import IfElse from './components/IfElse.svelte'
import Each from './components/Each.svelte'
import Await from './components/Await.svelte'
import DynamicClass from './components/DynamicClass.svelte'

const name = 'ashnamuh'

const ashnamuh = {
  age: 23
}

const jaemok = {
  name: 'Jaemok',
  age: 23
}

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
<Props name="ashnamuh" age={ashnamuh.age}></Props>
<Props {...jaemok}></Props>
<ArrayList></ArrayList>
<IfElse></IfElse>
<Each></Each>
<Await></Await>
<DynamicClass></DynamicClass>