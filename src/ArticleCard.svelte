<script>
    import {onMount} from 'svelte'
    let types = [ "social", "tech"]
    let titles = [
        "Justin Timberlake’s Big-Screen Reboot",
        "This is a small titile",
        "Biden inherited a rocky vaccine rollout, but the White House",
        "Angry Hedge Fund Billionaire Leon Cooperman Is Mad at GameStop",
        "The Second-Hardest Job in the World Is Up for Grabs",
        "Madeleine L’Engle’s Private Correspondence With Ahmad Rahman"
    ]

    let img
    let size = 400+Math.floor(Math.random()*100)

    // onMount(() => {
    //     img.style.backgroundImage = `url(https://picsum.photos/${size}`
    // })

    let type = types[Math.floor(Math.random()*types.length)]
    let title = titles[Math.floor(Math.random()*titles.length)]
</script>

<article class={type}>
    <div class="top">
        <div class="image" bind:this={img}></div>
    </div>
    <div class="bottom">
        <h3 class={type}>{type}</h3>
        <h2>{title}</h2>
        <p>23 Jan 2021</p>
    </div>
</article>

<style>
    article {
        display: inline-block;
        width: 18rem;
        padding: 1.5rem;
    }
    article.social {
        /* background-color: ivory; */
    }
    article.tech {
        /* background-color: aliceblue; */
    }

    .image {
        width: 100%;
        height: 9rem;
        border: 1px solid #000;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
    }

    .bottom {
        text-align: center;
        padding: 0 1.3rem;
    }
    h3 {
        text-transform: uppercase;
        font-weight: 400;
        font-size: 1.1rem;
        margin: 0;
        margin-top: 1.1rem;
    }
    h3.tech {
        margin-top: 1.25rem;
        font-size: 0.9rem;
        font-family: "Press Start 2P";
    }
    h3.social {
        font-family: Bungee Shade;
        font-weight: normal;
    }
    h2 {
        font-weight: 500;
        font-size: 1.3rem;
        line-height: 1.8rem;
        margin-bottom: 0.6rem;
        margin-top: 1.2rem;
    }
    p {
        letter-spacing: 0.1rem;
        text-transform: uppercase;
        font-size: 0.7rem;
        margin: 0;
        margin-top: 0.8rem;
        font-style: italic;
    }
</style>