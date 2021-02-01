<script>
	import Header from "./Header.svelte";
	import LongArticle from "./LongArticle.svelte";
	import ArticleCard from "./ArticleCard.svelte";
	import MainArticle from "./MainArticle.svelte";
</script>

<div class="container">
	<div class="header-wrapper">
		<!-- <Header /> -->
	</div>

	<main>
		<div class="articles-container">
			<div class="left">
				<h3>Trending</h3>
				<ArticleCard />
				<ArticleCard />
			</div>
			<div class="middle">
				<h3>Featured</h3>
				<MainArticle />
			</div>
			<div class="right">
				<h3>Evergreen</h3>
				<ArticleCard />
				<ArticleCard />
			</div>
		</div>

		<div class="todays-article-wrapper">
			<div class="heading-wrapper"><h3>Today's Articles</h3></div>
			<LongArticle index="1" />
			<LongArticle index="2" />
			<LongArticle index="3" />
			<LongArticle index="4" />
		</div>
	</main>
</div>

<style>
	.container {
		min-width: 300px;
		max-width: 1300px;
		width: 100%;
		margin: 0 auto;
		position: relative;
		overflow: hidden;
	}

	/* .header-wrapper {
		position: fixed;
		margin: 0 auto;
		width: 100%;
		min-width: 300px;
		max-width: 1300px;
		left: 0;
		right: 0;
		top: 0;
	} */

	main {
		/* margin-top: 12rem; */
	}

	.articles-container {
		display: flex;
		border-bottom: 1px solid #000;
	}
	h3 {
		margin: 0;
		margin-top: 2.2rem;
		font-size: 2rem;
		text-transform: capitalize;
		font-weight: 400;
		border-bottom: 1.3px solid #f00;
	}
	.left {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.middle {
		flex: 3;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.right {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.todays-article-wrapper {
		width: 100%;
		max-width: 1025px;
		margin: 0 auto;
	}
	.todays-article-wrapper .heading-wrapper {
		width: 100%;
		height: 8rem;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.todays-article-wrapper h3 {
		all: unset;
		font-size: 3rem;
		margin: 3rem 0 2rem 0;
		border-bottom: 1px solid #f00;
	}

	@media (max-width: 319px) {
        /* smartphones, iPhone, portrait 480x320 phones */
		.todays-article-wrapper h3 {
			font-size: 2rem;
		}
    }
    @media (max-width: 374px) {
        /* portrait e-readers (Nook/Kindle), smaller tablets @ 600 or @ 640 wide. */
    } 
    @media (max-width: 424px) {
        /* portrait tablets, portrait iPad, landscape e-readers, landscape 800x480 or 854x480 phones */
		.todays-article-wrapper {
			width: 100%;
		}

		.todays-article-wrapper h3 {
			font-size: 2.3rem;
			margin: 4rem 0 2rem 0;
		}
    }
    @media (max-width: 767px) {
        /* tablet, landscape iPad, lo-res laptops ands desktops */
		.todays-article-wrapper h3 {
			margin: 4rem 0 2rem 0;
		}
		.todays-article-wrapper {
			width: 100%;
		}
    }
    @media (max-width: 1023px) {
        /* big landscape tablets, laptops, and desktops */
		.container {
			max-width: 900px;
		}

		.articles-container {
			flex-wrap: wrap;
		}
		.articles-container .middle {
			order: 1;
			flex: 0 0 100%;
		}
		.articles-container .left {
			order: 2;
		}
		.articles-container .right {
			order: 3;
		}
    }
    @media (max-width: 1439px) {
        /* hi-res laptops and desktops */
    }
</style>
