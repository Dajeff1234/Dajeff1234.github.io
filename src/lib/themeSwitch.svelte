
<script>
    export let theme = true
</script>
<svelte:head>
    {#if theme}
  <style>:root {background: rgb(36, 36, 36);color: rgb(212, 212, 212);} .Button{color: rgb(212, 212, 212);}</style>
  {:else }
  <style>:root {background: rgb(235, 235, 235); color: black;}</style>
  {/if}

</svelte:head>
<li><button  class="Button" on:click="{() => theme = !theme}">theme</button></li>
<style>
    .Button{
        background:none;
        border:none;
        
    }
</style>