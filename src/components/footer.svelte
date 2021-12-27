<script>
    import CompSocial  from './social_component.svelte';
    import {socialinks} from './home/social-links';
</script>

<footer>
    <div>
        <a class="div-number" id="number1" href="tel:+51984135388">
            <i class="fas fa-phone-alt"/>
            <h5>984135388</h5>
        </a>
        <a class="div-number" id="number2" href="tel:+51954222499">
            <i class="fas fa-phone-alt"/>
            <h5>954222499</h5>
        </a>
    </div>
    <h4>
        Dios te trajo y nosotros te recibimos con amor
    </h4>
    <div class="div-social">
        {#each socialinks as sc}
            <a rel="nofollow noopener noreferrer" target="_blank" href={sc.URL}>
                <i class="fab {sc.icon}"/>
            </a>
        {/each}
    </div>
</footer>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Oswald:wght@600&display=swap");
    .div-number{ 
        margin-left: 5px;
        color: #fff;
        transition: color 1s;
        display: flex;
        flex-direction: row;
        align-items: center;
        text-decoration: none;
    }
    .fab{
        color: #fff;
        font-size: 30px;
        padding-right: 10px;
        padding-left: 10px;
        transition: color 1s;
    }
    .fa-facebook:hover{
        color: #5377F3;
        transition: color 1s;
    }
    .fa-instagram:hover{
        color: #E986D8;
        transition: color 1s;
    }
    h4{
        color: #fff;
        font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
    }
    h4,h5{
        font-size: 30px; 
    }
    .fas{
        margin-right: 5px;
        font-size: 25px;
    }
    .div-number:hover{
        color: rgba(148, 178, 185,0.3);
        transition: color 1s;
    }
    footer{
        padding:5px;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        bottom: 0;
        z-index: 1;
        height: 100%;
        background-color: #000;
    }
    .div-social{

        display: flex;
        flex-direction: row;
        justify-content: center;
        width: 10%;
    }
    @media only screen and (max-width: 888px){
        .div-social{
            display: flex;
            flex-direction: column;
            justify-content: center;
            width: 6%;
        }
        h5{
            font-size: 20px;
        }
    }
    @media only screen and (max-width: 799px){
        .div-social{
            display: flex;
            flex-direction: column;
            justify-content: center;
            width: 7%;
        }
        h4{
            font-size: 26px;
        }
    }
    @media only screen and (max-width: 713px){
        .div-number{
            display: none;
        }
        .div-social{
            display: none;
        }
        footer{
            padding:5px;
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: space-evenly;
            bottom: 0;
            z-index: 1;
            height: 100%;
            background-color: #000;
        }
        h4{
            font-size: 26px;
            text-align: start;
        }
    }
    @media only screen and (max-width: 512px){
        .div-number{
            display: none;
        }
        .div-social{
            display: none;
        }
        footer{
            padding:5px;
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: space-evenly;
            bottom: 0;
            z-index: 1;
            height: 100%;
            background-color: #000;
        }
        h4{
            font-size: 20px;
            text-align: start;
            transition: font-size 1s;
        }
    }
    @media only screen and (max-width: 400px){
        .div-number{
            display: none;
        }
        .div-social{
            display: none;
        }
        footer{
            padding:5px;
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: space-evenly;
            bottom: 0;
            z-index: 1;
            height: 100%;
            background-color: #000;
        }
        h4{
            font-size: 15px;
            text-align: start;
            transition: font-size 1s;
        }
    }
    @media only screen and (max-width: 300px){
        .div-number{
            display: none;
        }
        .div-social{
            display: none;
        }
        footer{
            padding:5px;
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: space-evenly;
            bottom: 0;
            z-index: 1;
            height: 100%;
            background-color: #000;
        }
        h4{
            font-size: 14px;
            text-align: start;
            transition: font-size 1s;
        }
    }
</style>
