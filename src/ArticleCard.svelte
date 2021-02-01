<script>
    let types = ["social", "tech"];
    let titles = [
        "Justin Timberlake’s Big-Screen Reboot",
        "This is a small titile",
        "Biden inherited a rocky vaccine rollout, but the White House",
        "Angry Hedge Fund Billionaire Leon Cooperman Is Mad at GameStop",
        "The Second-Hardest Job in the World Is Up for Grabs",
        "Madeleine L’Engle’s Private Correspondence With Ahmad Rahman",
    ];

    let type = types[Math.floor(Math.random() * types.length)];
    let title = titles[Math.floor(Math.random() * titles.length)];
</script>

<article class={type}>
    <div class="top">
        <div class="image" />
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
        width: 100%;
        min-width: 16rem;
        max-width: 18rem;
        padding: 20px;
        margin-bottom: 20px;
        background-color: rgb(255, 252, 238);
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
        padding: 20px;
        padding-bottom: 0;
    }
    h3 {
        text-transform: uppercase;
        font-weight: 400;
        font-size: 1rem;
        margin: 0;
    }
    h3.tech {
        font-family: "Press Start 2P";
    }
    h3.social {
        font-family: Bungee Shade;
    }
    h2 {
        font-weight: 500;
        font-size: 1.3rem;
        line-height: 1.8rem;
        margin: 20px 0;
    }
    p {
        letter-spacing: 0.1rem;
        text-transform: uppercase;
        font-size: 0.7rem;
        margin: 0;
        font-style: italic;
    }
</style>
