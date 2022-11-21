<script>
    import Dajeff1234 from "./icons/DAJEFF1234.svg"
    import ThemeButton from "./themeSwitch.svelte";
</script>

<nav>
    <div class = "nav-cont">
        <ul class="navTent">
            <ui><ThemeButton/></ui>
        </ul>
        <img src={Dajeff1234} alt="dajeff1234" class = "dajeff1234">
    </div>
</nav>
<style>
    
    .nav-cont{
        font-family: 'Montserrat', sans-serif !important;
        margin: 0px;
        background-color: rgb(86, 86, 86);
        padding: 2px !important;;
    }
    .navTent{
        
        display: inline-block ;
        list-style: none;
        text-align: center !important;
    }
    .dajeff1234{
        margin-top: 5.5px;
        width:200px;
        float: right;
    }
</style>
