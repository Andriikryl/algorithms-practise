<script>
  let valueNumber = "";
  let list = [];
  function addToList() {
    list = [...list, valueNumber];
    valueNumber = "";
  }
</script>

<section class="counter">
  <div class="container">
    <div>
      <p>{valueNumber}</p>
      <form on:submit|preventDefault>
        <div>
          <label for="input">type your number heare</label>
          <input bind:value={valueNumber} type="number" />
        </div>
        <button on:click={addToList}>add number</button>
      </form>
      <div>
        <ol>
          {#each list as item}
            <li>{item}</li>
          {/each}
        </ol>
      </div>
    </div>
  </div>
</section>
