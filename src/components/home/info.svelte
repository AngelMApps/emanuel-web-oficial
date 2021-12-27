<script>
  // your script goes here
</script>

<!-- markup (zero or more items) goes here -->

<div class="div-info">
  <p>
    Nuestra misión como iglesia es llevar el mensaje de salvación 
    y mostrar el amor de Dios a todas las personas. 
  </p>
  <img alt="logo" src="../images/logo.png"/>
</div>

  
<style>
  @import url("https://fonts.googleapis.com/css2?family=Oswald:wght@600&display=swap");
  div{
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
    height: 35rem;
    border-radius: 35px;
    padding: 2.5rem;
    margin-top: 6rem;
    background-color: rgba(129, 188, 218, 0.1);
    box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
  }
  p{
      color: #fff;
      text-align: center;
      font-size: 30px;
      font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
      padding-top: 2rem;
      font-weight: 200;
  }
  img{
    height: 20rem;
  }
  @media only screen and (max-width: 630px){
    p{
      color: #fff;
      text-align: center;
      font-size: 25px;
      font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
      padding-top: 2rem;
      font-weight: 200;
    }
  }
  @media only screen and (max-width: 491px){
    p{
      color: #fff;
      text-align: center;
      font-size: 25px;
      font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
      padding-top: 2rem;
      font-weight: 200;
    }
    img{
      height: 17rem;
    }
  }
  @media only screen and (max-width: 410px){
    p{
      color: #fff;
      text-align: center;
      font-size: 23px;
      font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
      padding-top: 2rem;
      font-weight: 200;
    }
    img{
      height: 13rem;
    }
  }
  @media only screen and (max-width: 331px){
    p{
      color: #fff;
      text-align: center;
      font-size: 20px;
      font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
      padding-top: 2rem;
      font-weight: 200;
    }
    img{
      height: 12rem;
    }
  }
</style>
