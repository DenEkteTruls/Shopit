<script>
    export let title = "";
    export let products = [];
    export let url = "";
</script>



<div class="container">
    <div class="left">
        <div id="image">
            <img src={url} alt="" id="icon"/>
        </div>
    </div>
    <div class="mid">
        <h1>{title}</h1>
        <p>{products.length} products</p>
    </div>
    <div class="right">
        >
    </div>
</div>



<style>
    .container {
        display: grid;
        grid-template-columns: 60px calc(80vw - 60px) calc(20vw - 60px);
        height: 70px;
        padding: 5px;
    }

    .mid {
        display: flex;
        justify-content: center; 
        flex-direction: column;
        gap: 4px;
        padding-left: 15px;
    }

    .right {
        display: flex;
        justify-content: center; 
        align-items: center;
        font-size: 25px;
        font-family: var(--font-regular);
        color: var(--darker-grey);
    }

    h1 {
        font-family: var(--font-semibold);
        font-size: 17px;
        margin: 0;
    }

    p {
        font-family: var(--font-regular);
        font-size: 15px;
        color: var(--dark-grey);
        margin: 0;
    }

    .left {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    #image {
        background-color: var(--background-orange);
        height: 60px;
        width: 60px;
        object-fit: cover;
        border-radius: 25px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    #icon {
        height: 28px;
        width: auto;
        object-fit: cover;
    }

</style>