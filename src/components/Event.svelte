<script>
const showAlert = () => alert('Hi!')

const clickGrandParent = () => console.log('clicked grand parent')
const clickParent = () => console.log('clicked parent')
const clickChild = () => console.log('clicked child')
</script>

<button on:click={showAlert}>함수 분리</button>

<button on:click={() => alert('Hello!')}>인라인 js</button>

<div class="grand-prent" on:click|capture={clickGrandParent}>
  <div class="parent" on:click|capture={clickParent}>
    <div class="child" on:click|capture={clickChild}>
      이벤트 캡쳐링
    </div>
  </div>
</div>

<div class="grand-prent" on:click={clickGrandParent}>
  <div class="parent" on:click={clickParent}>
    <div class="child" on:click={clickChild}>
      이벤트 버블링
    </div>
  </div>
</div>