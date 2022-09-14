<script>
    import List from './components/List.svelte';
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
        <List/>
        <p class="detail dark-grey">Recently created</p>
        <div class="recent">
            <List/>
            <List/>
            <List/>
            <List/>
        </div>
    </div>
    <div class="navbar-container">
    </div>
</div>


<style>
    .body {
        width: 100vw;
        height: 100vh;
        display: grid;
        grid-template-rows: 12.5vh 75vh 12.5vh;
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
        grid-template-rows: 30px 100px 30px calc(75vh - 160px);
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
</style>

