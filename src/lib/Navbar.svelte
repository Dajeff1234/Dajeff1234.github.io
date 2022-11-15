<script>
    export let theme = true
</script>
<style>
    
    .nav-cont{
        background-color: rgb(86, 86, 86);
        padding:2px;
    }
    .navTent{
        list-style: none;
    }
    .Button{
        background:none;
        border:none;
        
    }
</style>
<svelte:head>
    {#if theme == true}
  <style>:root {background: rgb(36, 36, 36);color: rgb(212, 212, 212);} .Button{color: rgb(212, 212, 212);}</style>
  {:else if theme == false}
  <style>:root {background: rgb(235, 235, 235);}</style>
  {/if}

</svelte:head>
<nav>
    <div class = "nav-cont">
        <ul class="navTent">
            <li><button  class="Button" on:click="{() => theme = !theme}">theme</button></li>
        </ul>
    </div>
</nav>
