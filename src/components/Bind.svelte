<script>
let name = ''

let selected = []

let selectedSkills = []

let favorite = ''

</script>

<select multiple bind:value={selected}>
  <option value="Vue">Vue</option>
  <option value="Angular">Angular</option>
  <option value="React">React</option>
  <option value="Svelte">Svelte</option>
</select>

<p>selected values are {selected}</p>
<input type="text" bind:value={name}>
<p>name is {name}</p>

<fieldset>
<legend>다음 중 능숙한 것을 모두 선택하세요.</legend>
<label><input type="checkbox" bind:group={selectedSkills} value="Git">Git</label>
<label><input type="checkbox" bind:group={selectedSkills} value="TDD">TDD</label>
<label><input type="checkbox" bind:group={selectedSkills} value="DDD">DDD</label>
<label><input type="checkbox" bind:group={selectedSkills} value="OOP">OOP</label>
<label><input type="checkbox" bind:group={selectedSkills} value="FP">FP</label>
</fieldset>

<p>능숙한 것들: {selectedSkills}</p>

<fieldset>
<legend>가장 관심있는 분야를 선택하세요.</legend>
<label><input type="radio" bind:group={favorite} value="풀스택">풀스택</label>
<label><input type="radio" bind:group={favorite} value="프론트엔드">프론트엔드</label>
<label><input type="radio" bind:group={favorite} value="백엔드">백엔드</label>
</fieldset>

<p>관심분야: {favorite}</p>