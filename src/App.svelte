<script>
  import { fly } from './transitions';
  import Navbar from "./lib/Navbar.svelte";
  import { onMount } from 'svelte';
  let ready = false;
  onMount(() => ready = true);
</script>
<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@200&display=swap" rel="stylesheet">
</svelte:head>
<style>
  
  :global(body) {
    margin: 0;
  }
  :root{
    font-family: 'Montserrat', sans-serif !important;
  }
  .welcom{
    padding-top: 20%;
    text-align: center;
    font-size: 50px;
  }
  .welcom2{
    text-align: center;
    font-size: 50px;
  }
</style>

<main>
  <Navbar/>
  {#if ready}
  <div class = "welcom" transition:fly={{ x: '500%' }}>welcom</div>
  {/if}
  <div class = "welcom2">to dajeff1234</div>
</main>