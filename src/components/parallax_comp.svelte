<script>
    export let iURL="";
    export let sHeight=40;
    export let sPadding=0;
    export let bright=0.2;
</script>

<section style="height: {sHeight}rem; background-image:url({iURL}); padding:{sPadding}px; filter:brightness({bright});" class="div_back"/>


<style>
    section{
        background: #fff fixed no-repeat 50% 50%;
        background-size: cover;
        left: 0;
        right: 0;
        top: 0;
        margin: 0;
        background-position: center;
    }
    .div_back{
        background-color: rgba(0,0,0,0.9);
        z-index:0; 
    }
</style>

