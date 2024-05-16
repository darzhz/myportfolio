<script>
    let salutation = "Full Stack Developer"
    import img from "./art11.png";
    let description = "Crafting digital experiences that leave a lasting impression - one line of code at a time"
    import FancyName from "./FancyName.svelte";
</script>
<div class="hero">
    <div class="text-content">
        <p class="salu">{salutation}</p>
        <!-- <h1 class="name">Darsh Shyam</h1> -->
        <!-- <FancyName /> -->
        <h1 class="name">Darsh Shyam</h1>
        <p class="desc">{description}</p>
        <div class="btns">
            <a  class="button" href='/#projects'>View Projects</a>
            <a class="button" href='https://drive.google.com/file/d/1FBL4UdLPD9-FCzxb-2Q34ZK-wYH_xwzD/view?usp=sharing'>Download Resume</a>
        </div>
    </div>
    <div class="content">
        <img src={img} alt="hero" />
    </div>
</div>
<!-- split the hero into two -->
<style>
    *{
        color: white;
    }
    .content img{
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 100%;
        height: 300px;
        object-fit: cover;
    }
    .hero {
        display: grid;
        grid-template-columns: 1fr 1fr;
        padding:10vh 0vh;
    }
    .name {
        font-size: 3rem;
        margin: 0;
    }
    .salu {
        font-size: 1.5rem;
        margin: 0;
        color: rgba(255, 255, 255, 0.7);
    }
    .text-content {
       text-align: left;
       padding: 20px;
    }

    .desc {
        font-size: 1.2rem;
        color: rgba(255, 255, 255, 0.7);
    }
    .desc::after {
        content: "";
        display: block;
        width: 50px;
        border-bottom: 2px solid white;
        margin-top: 0.5rem;
    }

    .btns {
        display: flex;
        gap: 1rem;
    }

    .button {
        padding: 0.5rem 1rem;
        border: none;
        border-radius: 5px;
        background: rgba(255, 255, 255, 0.1);
        color: white;
        cursor: pointer;
    }
    .button:hover {
        background: rgba(255, 255, 255, 0.2);
    }
    .button:active {
        background: rgba(255, 255, 255, 0.3);
    }
    .button:focus {
        outline: none;
    }
    .button:active {
        transform: scale(0.95);
    }
    .button {
        transition: all 0.3s ease;
    }
    a{
        text-decoration: none;
    }
    @media (max-width: 768px){
        .hero {
           grid-template-areas: "content content content" "text-content text-content text-content";
        }
        .text-content {
            text-align: center;
            grid-area: text-content;
        }
        .btns {
            justify-content: center;
        }
        .content {
            grid-area: content;
        }
        .content img{
            height: 500px;
        }
        .hero {
            padding: 1px 0vh;
        }
    }
</style>