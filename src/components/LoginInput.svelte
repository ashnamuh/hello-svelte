<script>
export let childFormData = {
  id: '',
  password: ''
}

</script>

<fieldset>
  <legend>로그인</legend>
  <label>
    <input type="text" bind:value={childFormData.id}>아이디
  </label>
  <label>
    <input type="password" bind:value={childFormData.password}>비밀번호
  </label>
</fieldset>
