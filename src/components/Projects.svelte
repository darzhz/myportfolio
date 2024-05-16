<script>
    import Card from "./Card.svelte";
    import data from "./projects.json"
    console.log(data)
</script>
<div class="title">
    <h1>My Projects</h1>
</div>
    <div class="showcase">
        {#each data.projects as project}
        <div class="card">
            <Card title={project.title} tech={project.tech} img={project.img} links={project.links}/>    
        </div>
        {/each}
    </div>

<style>
    .showcase{
        /* make a grid with 3 */
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 1rem;
        margin: auto;
    }
    .card {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .title{
        text-align: left;
        color: white;
        margin-top: 2rem;
        padding: 20px;
    }
    @media (min-width: 768px){
        .showcase{
            grid-template-columns: repeat(3, 1fr);
            gap: 0;
        }
    }
    
    @media (max-width: 550px){
        .showcase{
            grid-template-columns: 1fr;
        }
    }
</style>