<script>
    let counter = 9;
</script>



<div class="container">
    <div></div>
    <div></div>
    <div class="image"><img src="media/icons/cart.png" alt=""/><div class="counter">{counter}</div></div>
    <div></div>
    <div class="image"><img src="media/icons/profile.png" alt=""/></div>
</div>



<style>
    .container {
        width: 84%;
        height: 100%;
        display: grid;
        grid-template-columns: 20% 20% 20% 20% 20%;
        align-items: center;
        justify-content: center;
        margin: 0 auto;
    }

    .image {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    img {
        height: 40px;
        width: auto;
        object-fit: cover;
    }

    .counter {
        background-color: #8E5EED;
        width: 12px;
        height: 10px;
        border-radius: 5px;
        color: white;
        font-size: 8px;
        position: absolute;
        margin-left: 25px;
        margin-bottom: 16px;
        text-align: center;
        padding-top: 2px;
        border: 2px solid white;
        border-image: white; /* -webkit-linear-gradient(-90deg,#FEE4DC,#FEF6F3) 2 stretch; */
    }
</style>