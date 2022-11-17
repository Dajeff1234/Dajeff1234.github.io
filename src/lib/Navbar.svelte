<script>
    import ThemeButton from "./themeSwitch.svelte";
</script>

<nav>
    <div class = "nav-cont">
        <ul class="navTent">
            <ThemeButton/>
        </ul>
    </div>
</nav>
<style>
    
    .nav-cont{
        margin: 0px;
        background-color: rgb(86, 86, 86);
        padding:2px;
    }
    .navTent{
        list-style: none;
    }
</style>
