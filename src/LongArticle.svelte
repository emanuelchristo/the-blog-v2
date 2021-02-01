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
        width: 100%;
        display: flex;
        min-height: 15rem;
        padding: 30px;
        border-bottom: 1px solid #000;
    }

    .left {
        flex: 1;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    #slno {
        font-size: 2.1rem;
        margin: 5px 0;
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
        height: 100%;
        min-height: 12rem;
    }

    .right {
        flex: 8;
        padding: 20px;
    }
    h2 {
        font-weight: 600;
        font-size: 1.6rem;
        line-height: 2.1rem;
        margin: 0;
    }
    .right p {
        font-family: Jost;
        margin: 10px 0;
        text-indent: 2rem;
        letter-spacing: 0.06rem;
    }

    #date {
        all: unset;
        text-transform: uppercase;
        font-family: Roboto Mono;
        font-size: 0.8rem;
        font-style: italic;
    }

    @media (max-width: 1440px) {
		/* Laptop L */
	}
	@media (max-width: 1024px) {
		/* Laptop */
	}
	@media (max-width: 768px) {
		/* Tablet */
        article {
            flex-direction: column;
            text-align: center;
            max-width: 30rem;
            margin: 0 auto;
        }
        h2 {
            font-size: 1.7rem;
        }
        .right {
            padding-bottom: 0;
        }
        .right p {
            text-indent: 0;
        }
	}
	@media (max-width: 425px) {
		/* Mobile L */
	}
	@media (max-width: 375px) {
		/* Mobile M */
	}
	@media (max-width: 320px) {
		/* Mobile S */
	}
</style>
