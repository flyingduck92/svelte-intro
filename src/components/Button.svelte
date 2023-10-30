<script>
  export let count = 10
  export let handleClick = () => {
    count += 1
  }
</script>

<button on:click={handleClick}>Count: {count}</button>
