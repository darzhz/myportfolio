<script>
    export let tech = ["Nodejs", "Javascript", "Sqlite", "Prisma"];
    export let links = ["www.github.com", "www.linkedin.com"];
    export let img = "https://raw.githubusercontent.com/darzhz/Realnotes/main/assets/0.png";
    export let title = "Nodejs Project";
    const getDomain = (link) => {
        return link.split(".")[1];
    }
    const assignRandomColor = () => {
        let colors = ["#F01A4799", "#FCAF1799", "#3F5EBA99", "#00C85399", "#FFA70A99", "#9D38BD99", "#79554899", "#FFCC0099", "#4CAF5099", "#E91E6399", "#03A9F499", "#EC407A99"];
        return colors[Math.floor(Math.random() * colors.length)];
    }
</script>
<div class="card">
<div class="title">
    <h3>{title}</h3>
</div>
<div class="tags">
    {#each tech as tag}
        <div class="tag" style="background: {assignRandomColor()}">{tag}</div>
    {/each}
</div>
<div class="showcase">
<img src={img} alt="showcase" />
</div>
<div class="links">
{#each links as link }
    <span class="link"><a href={"http://"+link} >{getDomain(link)}</a></span>
{/each}
</div>
</div>
<style>
    .title{
        display: flex;
        justify-content: space-between;
    }
    .card{
        /* background: #333; */
        color: white;
        padding: 1rem;
        border-radius: 10px;
        /* margin: 1rem; */
        width: 300px;
    }
    .tags{
        display: flex;
        gap: 0.5rem;
        margin-bottom: 1rem;
    }
    .tag{
        padding: 0.5rem 1rem;
        color: white;
        border-radius: 15px;
        font-size: x-small;
        cursor: pointer;
        transition: transform 0.3s;
    }
    .tag:hover{
        transform: scale(1.1);
    }
    .links{
        display: flex;
        gap: 1rem;
        margin-top: 1rem;
    }
    .link{
        font-size: 1rem;
        margin-right: 0.2rem;
        cursor: pointer;
        transition: transform 0.3s;
        }
    .link:hover{
        transform: scale(1.1);
    }
    .showcase img{
        width: 100%;
        height: 200px;
        object-fit: cover;
        border-radius: 10px;
    }
    a{
        text-decoration: none;
        color: white;
        padding: 10px;
        border: dashed 1px white;
        border-radius: 15px;
    }
</style>