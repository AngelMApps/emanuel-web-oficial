<script>
// your script goes here
import Navbar from "../../components/Navbar.svelte";
</script>

<style>
/* your styles go here */
    main{
        position: absolute;
        top: 0;
        width: 100%;
        padding: 0;
        margin: 0;
        z-index: 0;
    }
    div{
        position: absolute;
        top: 10rem;
        bottom: 0;
        left: 0;
        right: 0;
        z-index:1;
        }
    h2{
        color: #fff;
        font-size: 30px;
    }
    section {
        background: #fff fixed no-repeat 50% 50%;
        background-size: cover;
        left: 0;
        right: 0;
        top: 0;
        margin: 0;
        background-position: center;
        background-repeat: no-repeat;
    }
    .background__top {
        height: 40rem;
        padding: 10px;
        background-color: rgba(0, 0, 0, 1);
        background-image: url("../../../static/images/fondo4.jpg");
        filter: brightness(0.09);
        z-index: 0;
    }

</style>

<Navbar/>
<main>
    <div>
         <h2>Contactos</h2>
    </div>

    <section class="background__top"/>
</main>

<!-- markup (zero or more items) goes here
    <div class="div-past">
        <h2>Pastores</h2>
        <div class="div-past-info">
            <h3>Susi Huamanchay</h3>
             <img alt="logo" src="../images/pastores.svg"/>
            <h3>Angel Mora</h3>
         </div>
    </div>
    -->
