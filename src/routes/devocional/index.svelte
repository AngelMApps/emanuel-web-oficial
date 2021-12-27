<script>
    import CompParallax from '../../components/parallax_comp.svelte';
    import Footer from '../../components/footer.svelte';
    import Navbar from '../../components/Navbar.svelte';
</script>
<Navbar/>
<main>
    <div class="container-text">
        <h1>Devocional</h1>
        <hr/>
        <div class="parraf-cont">
            <p>" Dios mío, ¡tú eres mi Dios! Yo te buscaré de madrugada.<br/>
                Mi alma desfallece de sed por ti; mi ser entero te busca<br/> 
                con ansias ... " (Salmos 63:1)
            </p>
        </div>
    </div>
    <CompParallax iURL='../images/cDevo.png' sHeight=47/>
    <div class="div div-info">
        <h3>¿Qué es el tiempo de Devocional?</h3>
        <p>Es el tiempo que le entregamos a <strong>Dios</strong> para que él nos llene de fuerzas
            y <br/> así poder caminar firmes en cada situación que pueda ocurrirnos en el día.<br/>
        </p>
    </div>
    <CompParallax iURL='../images/fondo6.png' bright=0.1 />
    
    <div class="div div-info">
        <p>Te invitamos a nuestras reuniones de <strong>DEVOCIONAL</strong><br/>
            transmitidas en vivo de Lunes a Domingo.
        </p>
        <h5>desde las 6:00am hasta las 7:00am</h5>
    </div>
    <CompParallax iURL='../images/cDevo.png' />
    <Footer/>
</main>

<style>
    main{
      position: absolute;
        top: 0;
        width: 100%;
        padding: 0;
        margin: 0;
        z-index: 0;
    }
    .parraf-cont{
        width: 50rem;
    }
    .container-text {
    position: absolute;
    display: flex;
    flex-direction: column;
    align-items: center;
    top: 250px;
    left: 0;
    right: 0;
    z-index: 1;
    }
    .div{
      display:flex;
      flex-direction:column;
      justify-content:center;
      align-items: center;
      
      
    }
    .div-info{
    left: 15%;
    right: 15%;
    position: absolute;
    z-index: 1;
    height: 20rem;
    border-radius: 35px;
    padding: 2.5rem;
    margin-top: 10rem;
    background-color: rgba(129, 188, 218, 0.1);
    box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
    }
    hr{
        margin-top: 1rem;
        background-color: #fff;
        border: none;
        width: 10rem;
        height: 0.2rem;
    }
    h1 {
    margin: 0;
    color: #fff;
    font-size: 90pt;
    font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
    }
    p{
      color: #fff;
      margin-top: 1rem;
      font-size: 20pt;
      text-align: center;
      line-height: 2rem;
  }
  h3{
    margin: 0;
    color: #fff;
    font-size: 30pt;
    font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
  }
  h5{
      margin-top: 1rem;
      font-size: 25px;
      color: #A3B9F9;
  }
</style>



