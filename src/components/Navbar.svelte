<script>
    import { routes } from "./routes";
    import {meetLinks} from "./meeting_links"
    let sReuLinks=false;
    let y=0;
    let showReuLinks = () =>{
        sReuLinks = !sReuLinks;
    };
</script>
<svelte:window bind:scrollY={y}/>
<!-- markup (zero or more items) goes here nColor === 0 -->
<nav class={ y >= 200 ? "blur_nav" : "transparent_nav"}>
  <div class="nav-div">
    <a class="title" href={routes[0].route}>{routes[0].name}</a>
  </div>
</nav>
<ul class={sReuLinks ? "sidenav":"no_sidebar"}>
    {#each meetLinks as mt }
        <li on:click={showReuLinks}><a href={mt.route}>{mt.name}</a></li>
            <hr/>
        <hr/>
    {/each}
</ul>
<style>
    @import url("https://fonts.googleapis.com/css2?family=Oswald:wght@600&display=swap");
    @import url("https://fonts.googleapis.com/css2?family=Lobster&display=swap");
    nav {
        z-index: 2;
        position: fixed;
        top: 0;
        margin: 0;
        padding: 0;
        left: 0;
        right: 0;
        height: 4rem;
    }
    hr{
        border: none;
        width: 100%;
        height: 0.05rem;
        background-color: rgba(255,255,255,0.1);
    }

    .sidenav{
        position: fixed;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 10rem;
        background:rgba(14, 15, 18,1);
        height: 20rem;
        backdrop-filter: blur(200px);
        top: 4rem;
        left: calc(50% + 13.5rem);
        z-index: 2;
    }
    .sidenav a{
        padding: 5px;
        font-size: 14px;
        text-align: center;
        font-family: Helvetica, sans-serif, Arial;
        text-transform: uppercase;
    }
    .transparent_nav {
        background: transparent;
    }
    .blur_nav {
        background: rgba(0, 0, 0, 0.7);
        backdrop-filter: blur(200px);
     }
     .nav-div {
        padding: 10px 5px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
     }
     .title {
        font-size: 35px;
        font-family: "Lobster", "Oswald", Helvetica, sans-serif, Arial, sans-serif;
     }
     
    
    a{
        text-decoration: none;
        color: #fff;
        transition: color 1s;
    }
    
    a:hover {
        color: rgba(131, 152, 223,0.8);
        transition: color 1s;
        cursor: pointer;
    }
   
    ul {
    padding: 0;
    display: flex;
    flex-direction: row;
    width: 40%;
    height: 3rem;
    margin: 0;
    justify-content: space-evenly;
    align-items: center;
    list-style: none;
  }
  
    @media only screen and (max-width: 680px){
        .nav-div {
            padding: 10px 5px;
            display: flex;
            flex-direction: row;
            justify-content: center;
        }
    }
</style>
