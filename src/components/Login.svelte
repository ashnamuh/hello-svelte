<script>
import LoginInput from './LoginInput.svelte'

let formData = {
  id: '',
  password: ''
}

</script>

<h1>로그인 페이지</h1>
<LoginInput bind:childFormData={formData}></LoginInput>

아이디 입력값 : {formData.id}
비밀번호 입력값 : {formData.password}
