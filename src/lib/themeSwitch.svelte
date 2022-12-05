
<script>
    import { transition_in } from "svelte/internal";



    export let theme = true
    
    /*$: if (typeof document == 'object') {
        document.documentElement.classList.toggle('dark', theme)
    }*/
</script>
<svelte:head>
    {#if theme}
  <style>
        :root{
        transition: 1s;
        background: rgb(235, 235, 235); 
        color: black;
    }
        
    .Button{
        transition: 1s;
        font-family: 'Montserrat', sans-serif;
        background:none;
        border:none;
        color: rgb(212, 212, 212);
        
    }
    .newSection{
    transition: 1s;
    background-color: rgb(203, 203, 203);
    text-align: center;
    padding-bottom:55%;
  }
  .stuff{
    transition:1s !important;
  }
    </style>
  {:else }
    <style>
    :root {
        font-family: 'Montserrat', sans-serif !important;
        transition: 1s;
        background: rgb(36, 36, 36);
        color: rgb(212, 212, 212);
    } 
    .Button{
        transition: 1s;
        font-family: 'Montserrat', sans-serif;
        background:none;
        border:none;
        color: rgb(212, 212, 212);
        
    }
    
  .newSection{
    transition:1s;
    background-color: rgb(65, 65, 65) !important;
    text-align: center;
    padding-bottom:55%;
    }
    </style>
  {/if}

</svelte:head>

<li><button  class="Button" on:click="{() => theme = !theme}">theme</button></li>
<style>

    





</style>