<script>
    export let index;
</script>

<article>
    <div class="left">
        <p id="slno">{index}.</p>
    </div>
    <div class="middle">
        <div class="image" />
    </div>
    <div class="right">
        <div class="top">
            <h2>
                This is a very lengthy title for seeing how it looks. Ok? Lorem
                Epsom this is a good title.
            </h2>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor
                in repreh
            </p>
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
        padding: 1.5rem;
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
        min-height: 12rem;
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

    #date {
        all: unset;
        text-transform: uppercase;
        font-family: Roboto Mono;
        font-size: 0.8rem;
        font-style: italic;
    }

    @media (max-width: 319px) {
        /* smartphones, iPhone, portrait 480x320 phones */
    }
    @media (max-width: 374px) {
        /* portrait e-readers (Nook/Kindle), smaller tablets @ 600 or @ 640 wide. */
    } 
    @media (max-width: 424px) {
        /* portrait tablets, portrait iPad, landscape e-readers, landscape 800x480 or 854x480 phones */

    }
    @media (max-width: 767px) {
        /* tablet, landscape iPad, lo-res laptops ands desktops */
        article {
            flex-direction: column;
            padding: 3rem 1.8rem;
            text-align: center;
            max-width: 30rem;
            margin: 0 auto;
        }
        .right {
            padding-bottom: 0;
        }
    }
    @media (max-width: 1023px) {
        /* big landscape tablets, laptops, and desktops */
    }
    @media (max-width: 1439px) {
        /* hi-res laptops and desktops */
    }
</style>
