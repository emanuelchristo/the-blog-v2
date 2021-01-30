<script>
    export let index
</script>

<article>
    <div class="left">
        <p id="slno">{index}.</p>
    </div>
    <div class="middle">
        <div class="image"></div>
    </div>
    <div class="right">
        <div class="top">
            <h2>This is a very lengthy title for seeing how it looks. Ok? Lorem Epsom this is a good title.</h2>
            <p>    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in repreh</p>
        </div>
        <div class="bottom">
            <p id="date">12 Jan 2021</p>
        </div>
    </div>
</article>

<style>
    article {
        display: flex;
        min-height: 15rem;
        padding: 1rem;
        border-bottom: 1px solid #000;
    }

    .left {
        flex: 1;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    #slno {
        font-size: 2.3rem;
    }

    .middle {
        flex: 5;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .image {
        border: 1px solid #000;
        width: 100%;
        height: 86%;
    }

    .right {
        flex: 8;
        padding: 1.3rem;
    }
    h2 {
        font-weight: 600;
        font-size: 1.6rem;
        line-height: 2.45rem;
        margin: 0;
    }
    .right p {
        margin: 0.5rem 0;
        text-indent: 2rem;
        letter-spacing: 0.09rem;
    }

    .bottom {
        
    }
    #date {
        all: unset;
        text-transform: uppercase;
        font-family: Roboto Mono;
        font-size: 0.8rem;
        font-style: italic;
    }
 
</style>