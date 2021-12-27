<script>
    import {meetLinks} from '../meeting_links';
</script>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Oswald:wght@600&display=swap");
    .div-info {
        left: 15%;
        right: 15%;
        position: absolute;
        z-index: 1;
        height: 50rem;
        border-radius: 35px;
        padding: 2.5rem;
        margin-top: 6rem;
        background-color: rgba(129, 188, 218, 0);
        box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
    }
    p {
        color: #fff;
        text-align: center;
        font-size: 40px;
        font-weight: 200;
        font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
    }
    ul{
        padding: 0;
        list-style: none;
        width: 100%;
    }
    
    strong{
        text-decoration: none;
        font-size: 30px;
        text-align: center;
        font-weight: 200;
        font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
        cursor: pointer;
    }
    button{
        background-color: rgb(56, 138, 204);
    }
    .accordion-item{
        background-color: rgba(56, 126, 173, 0.71);
    }
    .accordion-body{
        text-align: center;
        font-size: 30px;
        color: #dbf0ff;
    }
    .div-title{
        background-color: transparent;
    }
    @media only screen and (max-width: 609px){
        .accordion-body{
            text-align: center;
            font-size: 25px;
            color: #dbf0ff;
        }
    }
    @media only screen and (max-width: 560px){
        .accordion-body{
            text-align: center;
            font-size: 20px;
            color: #dbf0ff;
        }
    }
    @media only screen and (max-width: 468px){
        .accordion-body{
            text-align: center;
            font-size: 17px;
            color: #dbf0ff;
        }
    }
    @media only screen and (max-width: 434px){
        strong{
            text-decoration: none;
            font-size: 26px;
            text-align: start;
            font-weight: 200;
            font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
            cursor: pointer;
        }
    }
    @media only screen and (max-width: 400px){
        .div-info {
            left: 15%;
            right: 15%;
            position: absolute;
            z-index: 1;
            height: 47rem;
            border-radius: 35px;
            padding: 2rem 1rem 2rem 1rem;
            margin-top: 6rem;
            background-color: rgba(129, 188, 218, 0);
            box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
        }
        strong{
            text-decoration: none;
            font-size: 22px;
            text-align: start;
            font-weight: 200;
            font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
            cursor: pointer;
        }
    }
    @media only screen and (max-width: 373px){
        p {
            color: #fff;
            text-align: center;
            font-size: 30px;
            font-weight: 200;
            font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
        }
        .div-info {
            left: 15%;
            right: 15%;
            position: absolute;
            z-index: 1;
            height: 47rem;
            border-radius: 35px;
            padding: 2rem 1rem 2rem 1rem;
            margin-top: 6rem;
            background-color: rgba(129, 188, 218, 0);
            box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
        }
        strong{
            text-decoration: none;
            font-size: 20px;
            text-align: start;
            font-weight: 200;
            font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
            cursor: pointer;
        }
    }
    @media only screen and (max-width: 340px){
        p {
            color: #fff;
            text-align: center;
            font-size: 27px;
            font-weight: 200;
            font-family: "Oswald", Helvetica, sans-serif, Arial, sans-serif;
        }
    }
</style>
<!-- class={ y >= 200 ? "blur_nav" : "transparent_nav"}-->
<main>
    <div class=" div-info accordion accordion-flush" id="accordionFlushExample">
        <div class="div-title">
            <p>
                Nuestras Reuniones
            </p>
        </div>
        <ul>
            {#each meetLinks as mt}
                    <div class="accordion-item">
                        <h2 class="accordion-header" id="flush-heading{mt.index}">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#flush-collapse{mt.index}" aria-expanded="false" aria-controls="flush-collapse{mt.index}">
                                <strong>{mt.name}</strong>
                            </button>
                        </h2>
                        <div id="flush-collapse{mt.index}" class="accordion-collapse collapse" aria-labelledby="flush-heading{mt.index}" data-bs-parent="#accordionFlushExample">
                            <div class="accordion-body">{mt.description}.</div>
                        </div>
                        <!--  <strong on:click={selectCulto}>{mt.name}</strong>   <a href={mt.route}>{mt.name}</a>-->
                    </div>
                    <br/>
            {/each}
        </ul>

        <!--<img alt="logo" src="../images/logo.png"/> -->

    </div>
</main>