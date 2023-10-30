<script>
  import { onDestroy } from 'svelte'
  import { count } from './stores/stores.js'
  import Button from './components/Button.svelte'
  import Resetter from './components/Resetter.svelte'
  let name = ''

  const increment = () => {
    $count += 1
  }
</script>

<main>
  <h1>Hello {name}! {$count}</h1>
  <form action="">
    <input type="text" bind:value={name} />
  </form>

  <Button count={$count} handleClick={increment} />
  <Resetter />
</main>
