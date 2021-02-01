<script>
</script>

<header>
    <div class="top">
        <div class="left">
            <div class="content-wrapper">
                <p id="time">12:34 am</p>
                <p id="date">friday, 30 Jan 2021</p>
                <button>SUBSCRIBE</button>
            </div>
        </div>
        <div class="middle">
            <h1>The Blog</h1>
        </div>
        <div class="right">
            <div class="content-wrapper">
                <h3>email</h3>
                <h3>github</h3>
                <h3>instagram</h3>
            </div>
        </div>
    </div>
    <div class="bottom">
        <h2 id="all">ALL</h2>
        <h2 id="social">SOCIAL</h2>
        <h2 id="tech">TECH</h2>
    </div>
</header>

<style>
    header {
        background-color: #fff;
    }
    .top {
        display: flex;
        width: 100%;
    }

    .left {
        flex: 1;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: flex-start;
        padding: 1.8rem;
    }

    button {
        font-size: 1rem;
        font-family: Bodoi Moda;
        padding: 0.5rem 0.6rem;
        border: none;
        background: #ff0000;
        color: #fff;
        margin: 0.1rem 0;
        font-weight: 700;
        letter-spacing: 0.06rem;
    }
    p {
        font-size: 0.8rem;
        letter-spacing: 0.09rem;
        text-transform: uppercase;
        margin: 0.2rem 0;
    }
    #date {
        font-weight: 700;
    }

    .right {
        height: 100%;
        flex: 1;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        text-align: right;
        padding: 1.8rem;
    }
    .right h3 {
        margin: 0.15rem 0;
        font-size: 0.9rem;
        text-transform: uppercase;
    }

    .middle {
        height: 100%;
        flex: 3;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    h1 {
        font-size: 3rem;
        text-decoration: underline wavy pink;
        text-decoration-thickness: 0.15rem;
    }

    .bottom {
        border-top: 1px solid #000;
        border-bottom: 1px solid #000;
        height: 3rem;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        position: -webkit-sticky;
        position: sticky;
        top: 0;
    }
    h2 {
        font-size: 1.3rem;
        margin: 0 1rem;
    }
    #social {
        font-family: Bungee Shade;
    }
    #tech {
        font-family: "Press Start 2P";
    }


	@media (max-width: 1439px) {
		/* Laptop L */
	}
	@media (max-width: 1023px) {
		/* Laptop */
	}
	@media (max-width: 767px) {
		/* Tablet */
        .top .left, .top .right {
            display: none;
        }
        .top {
            height: 6rem;
        }
        h1 {
            font-size: 2rem;
        }
	}
	@media (max-width: 424px) {
		/* Mobile L */
	}
	@media (max-width: 374px) {
		/* Mobile M */
	}
	@media (max-width: 319px) {
		/* Mobile S */
	}
</style>
