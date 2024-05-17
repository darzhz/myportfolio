<script>
    
</script>
<div class="nav">
    <div class="logo"><p>DARZH</p></div>
    <div class="links">
        <a class="link " href="#">Home</a>
        <a class="link " href="#projects">Projects</a>
        <a class="link " href="#contact">Contacts</a>
    </div>
</div>
<style>
    .nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1rem;
        background: rgba( 255, 255, 255, 0.1 );
        backdrop-filter: blur( 1.5px );
        -webkit-backdrop-filter: blur( 1.5px );
        border-radius: 10px;
        border: 1px solid rgba( 255, 255, 255, 0.18 );
        color: white;
        width: 90vw;
        gap: 50%;
        position: relative;
    }
    .link{
        font-size: 1rem;
        margin-right: 1rem;
        cursor: pointer;
        font-family: 'satoshi-light',sans-serif;
        text-decoration: none;
        color: white;
    }
    .logo {
        font-size: 1.5rem;
    }
    @media (max-width: 768px){
        .nav {
            gap: 25px;
            margin-top: 3vh;
        }
    }
</style>