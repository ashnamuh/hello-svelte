<script>
  const username = 'ashnamuh'
</script>

<div>
  <slot name="header" username={username}>헤더를 주입해주세요!</slot>
  <section>
    제 이름은 {username}입니다.
    저는 개발자입니다:)
  </section>
  <slot name="footer">푸터를 주입해주세요!</slot>
</div>