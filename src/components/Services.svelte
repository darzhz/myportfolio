<script>
  import { fly } from "svelte/transition";

    let services = [
        {
            title: 'Web Development',
            description: 'I specialize in building responsive, user-friendly websites that are both visually appealing and functional. I have experience with a variety of web technologies, including HTML, CSS, JavaScript, and React.'
        },
        {
            title: 'Mobile Development',
            description: 'I have experience developing mobile applications for both iOS and Android devices. I am proficient in using tools such as React Native and Flutter to create cross-platform mobile apps.'
        },
        {
            title: 'Machine Learning',
            description: 'I have a strong background in machine learning and artificial intelligence. I have experience working with popular machine learning libraries such as TensorFlow and Pytorch.'
        },
        {
            title: 'IoT Development',
            description: 'I have experience developing Internet of Things (IoT) applications. I have worked with a variety of IoT devices and platforms, including Arduino, Raspberry Pi, and NodeMCU.'
        }
    ];
</script>
<h1>Services</h1>
<div class="services">
    {#each services as service}
        <div class="service">
            <h2>{service.title}</h2>
            <p>{service.description}</p>
        </div>
    {/each}
</div>
<style>
    h1{
        color: white;
        text-align: center;
        margin: 20px;
        font-family: 'satoshi-regular',sans-serif;
    }
    .services{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 20px;
        padding: 20px;
        justify-content: center;
    }
    .service:hover{
        background: rgba(255, 255, 255, 0.2);
        transform: scale(1.05);
        cursor: pointer;
    }
    .service{
        background: rgba(255, 255, 255, 0.1);
        padding: 20px;
        border-radius: 10px;
        color: white;
        transition: all 0.3s ease-in-out;

    }
    .service h2{
        font-size: 1.5rem;
        margin: 0;
        font-family: 'satoshi-regular',sans-serif;
    }
    .service p{
        font-size: 1rem;
        color: rgba(255, 255, 255, 0.7);
        text-align: justify;
        /* font-family: 'satoshi-light',sans-serif; */

    }
</style>