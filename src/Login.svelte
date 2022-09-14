<script>
    function login()
    {
        var email = document.getElementById("email").value;
        var password = document.getElementById("passwd").value;
        console.log(email, password);
    }


    function register()
    {
        
    }
</script>


<div class="body">
    <div class="container">
        <img src="#" alt="" id="logo"/>
        <h1 id="title">Velkommen til <b id="bold">Shopit</b></h1>
        <p class="detail">Logg inn med epost og passord</p>
        <div class="login-container">
            <input type="email" placeholder="E-post" id="email"/>
            <input type="password" placeholder="Passord" id="passwd"/>
            <a href="#"><p id="fot">Glemt passordet?</p></a>
            <button class="button" on:click={() => {login()}}>Logg Inn</button>
            <button class="button" on:click={() => {register()}}>Opprett Bruker</button>
        </div>
    </div>
</div>



<style>

    .body {
        width: 100vw;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .container {
        margin-top: -20%;
        display: flex;
        flex-direction: column;
        max-width: 500px;
        justify-content: center;
        align-items: center;
        text-align: center;
    }

    #title {
        font-size: 40px;
        font-family: var(--font-thin-italic);
        margin-bottom: 30px;
        max-width: 90%;
        text-align: center;
    }

    #bold {
        font-family: var(--font-bold-italic);
    }

    .detail {
        font-size: 15px;
        font-family: var(--font-semibold);
    }

    .login-container {
        display: flex;
        flex-direction: column;
        width: 80%;
        padding: 1.25%;

    }

    input {
        height: 35px;
        margin-top: 7px;
        border: 1px solid var(--dark-grey);
        border-radius: 10px;
        padding: 2px 10px;
        font-family: var(--font-semibold);
        font-size: 15px;
    }

    input:focus {
        border-color: var(--grey);
        outline: 3px solid var(--lightyellow);
    }

    .button {
        height: 40px;
        border: none;
        border-radius: 10px;
        background-color: var(--yellow);
        color: white;
        font-family: var(--font-bold);
        font-size: 16px;
        cursor: pointer;
        width: 100%;
        margin: 4px 0;
        transition: background-color .4s ease-in-out;
        user-select: none;
    }

    .button:hover {
        background-color: var(--lightyellow);
    }

    #fot {
        color: var(--dark-grey);
        font-size: 12px;
        font-family: var(--font-semibold);
        margin: 6px  0 8px 4px;
        text-align: left;
    }
</style>