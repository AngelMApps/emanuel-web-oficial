<script>
    // your script goes here
</script>

<style>
    /* your styles go here */
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
    .div-number{ 
        margin-left: 5px;
        color: #fff;
        transition: color 1s;
        display: flex;
        flex-direction: row;
        align-items: center;
        text-decoration: none;
    }
    h5{
        font-size: 30px; 
    }
    .fas{
        margin-right: 5px;
        font-size: 25px;
    }
</style>

<!-- markup (zero or more items) goes here -->
<div class="div-info">
    <a class="div-number" id="number1" href="tel:+51984135388">
        <i class="fas fa-phone-alt"/>
        <h5>984135388</h5>
    </a>
    <a class="div-number" id="number2" href="tel:+51954222499">
        <i class="fas fa-phone-alt"/>
        <h5>954222499</h5>
    </a>
</div>