<script>
  import favicon from './lib/icons/f3.ico'
  import { fly } from './transitions';
  import Navbar from "./lib/Navbar.svelte";
  import { onMount } from 'svelte';
  let ready = false;
  onMount(() => ready = true);
  let ready2 = false;
</script>
<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@200&display=swap" rel="stylesheet">
  <link rel="icon" type="image/x-icon" href="{favicon}">
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
  main{
    padding-bottom: 25%;
  }
  
  
</style>

<main>
  <Navbar/>
  {#if ready}
  <div class = "welcom" transition:fly={{ x: '200%' }}>welcome</div>
  {/if}
  {#if ready}
  <div class = "welcom2" transition:fly={{ y: '600%' }}>to dajeff1234</div>
  {/if}
</main>
<div class="newSection">
  <div class = stuff>
    hello
  </div>
 
</div>