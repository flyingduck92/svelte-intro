<script>
  import { count } from '../stores/stores'

  const reset = () => {
    $count = 0
  }
</script>

<button on:click={reset}>Reset</button>
