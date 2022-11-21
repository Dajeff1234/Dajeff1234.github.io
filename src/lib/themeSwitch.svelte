
<script>

    export let theme = true
    
    $: if (typeof document == 'object') {
        document.documentElement.classList.toggle('dark', theme)
    }
</script>
<!-- <svelte:head>
    {#if theme}
  <style>
        :root {
            background: rgb(36, 36, 36);
            color: rgb(212, 212, 212);
        } 
        .Button{
            color: rgb(212, 212, 212);
        }
    </style>
  {:else }
    <style>
    :root {
        background: rgb(235, 235, 235); 
        color: black;
        } 
        .nav-cont{
            background-color: rgb(209, 209, 209) !important;
        }
    </style>
  {/if}

</svelte:head> -->

<li><button  class="Button" on:click="{() => theme = !theme}">theme</button></li>
<style>

    :root {
        font-family: 'Montserrat', sans-serif !important;
        transition: 1s;
        background: rgb(36, 36, 36);
        color: rgb(212, 212, 212);
    }

    :root.dark {
        background: rgb(235, 235, 235); 
        color: black;
    }

    .dark .nav-cont {
        transition: 1s;
        background-color: rgb(209, 209, 209) !important;
    }


    .Button{
        font-family: 'Montserrat', sans-serif;
        background:none;
        border:none;
        color: rgb(212, 212, 212);
        
    }
</style>