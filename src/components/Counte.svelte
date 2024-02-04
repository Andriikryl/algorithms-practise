<script>
  let count = 0;
  function dicriment() {
    count = count + 1;
  }
</script>

<section class="counter">
  <div class="container">
    <div>
      <h3>counter</h3>
      <h2>{count}</h2>
      <button on:click={dicriment}>dincrement</button>
    </div>
  </div>
</section>
