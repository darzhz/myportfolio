<div class="nav">
    <div class="logo">DARZH</div>
    <div class="links">
        <span class="link oswald">Home</span>
        <span class="link oswald">Projects</span>
        <span class="link oswald">Contacts</span>
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
        width: 80vw;
        gap: 50%;
    }
    .link{
        font-size: 1rem;
        margin-right: 1rem;
        cursor: pointer;
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