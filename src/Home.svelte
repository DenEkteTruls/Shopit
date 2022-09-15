<script>
    import List from './components/List.svelte';
    import Navbar from './components/Navbar.svelte';
</script>


<div class="body">
    <div class="top">
        <div></div>
        <h1 id="title">Shopping lists</h1>
        <div id="profile-image">
            <img src="media/profile-image.jpg" alt="">
        </div>
    </div>
    <div class="list-container">
        <p class="detail dark-grey">Our recommendations</p>
        <List title="Fruits list" products={[1, 2, 3, 4, 5]} url="https://static.vecteezy.com/system/resources/previews/001/208/675/original/banana-png.png"/>
        <p class="detail dark-grey">Recently created</p>
        <div class="recent">
            <List title="Morning breakfast" products={[1, 2, 3, 4, 5, 6]} url="https://cdn-icons-png.flaticon.com/512/4241/4241664.png"/>
            <List/>
            <List/>
            <List/>
        </div>
    </div>
    <div class="button-container">
        <button id="listbutton">Create new list</button>
    </div>
    <Navbar/>
</div>


<style>
    .body {
        width: 100vw;
        height: 100vh;
        display: grid;
        grid-template-rows: 12.5vh 69.5vh 10vh 8vh;
    }

    .top {
        display: grid;
        grid-template-columns: 15vw 70vw 15vw;

    }

    #title {
        display: flex;
        justify-content: center;
        align-items: center;
        font-family: var(--font-bold);
        font-size: 18px;
    }

    #profile-image {
        display: flex;
        border-radius: 100%;
        justify-content: center;
        align-items: center;
        padding-right: 40%;
    }

    #profile-image > img {
        width: 45px;
        height: auto;
        object-fit: cover;
        border-radius: 100%;
    }
    
    .list-container {
        width: 100vw;
        padding: 0 6%;
        display: grid;
        grid-template-rows: 30px 100px 30px 69.5vh;
    }

    .detail {
        font-family: var(--font-regular);
        font-size: 15px;
        letter-spacing: 0.4px;
        margin: 0;
        margin-left: 2%;
    }

    .dark-grey {
        color: var(--dark-grey);
    }

    .button-container {
        width: 100vw;
        padding: auto 6%;
        margin: 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: 5%;
    }

    #listbutton {
        height: 100%;
        max-height: 60px;
        min-height: 50px;
        width: 84%;
        border: none;
        border-radius: 40px;
        background-color: var(--yellow);
        color: white;
        font-family: var(--font-regular);
        font-size: 18px;
        box-shadow: 0px 10px 35px var(--lightyellow);
    }

</style>

