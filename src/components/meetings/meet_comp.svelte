<script >
    import CompParallax from '../parallax_comp.svelte';
    export let iTitle="";
    export let iURL="";
    export let mt=0;
</script>

<main>
    <div class="container-devocional">
        <h4 style="margin-top: {mt}rem;">{iTitle}</h4>
    </div>
    <CompParallax iURL={iURL} sHeight=40 sPadding=10 bright=0.2/> 
</main>

<style>
    main{
        width: 100%;
    }
    .container-devocional{
        width: 100%;
        position: absolute;
        display: flex;
        flex-direction: column;
        align-items: center;
        top: 0;
        left: 0;
        right: 0;
        z-index: 1;
        line-height: 2pt;
    }
    h4{
        color: #fff;
    }
</style>
