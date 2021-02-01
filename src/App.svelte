<script>
	import Header from "./Header.svelte";
	import LongArticle from "./LongArticle.svelte";
	import ArticleCard from "./ArticleCard.svelte";
	import MainArticle from "./MainArticle.svelte";
</script>

<div class="container">
	<div class="header-wrapper">
		<Header />
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
		max-width: 1200px;
		width: 100%;
		padding: 0 20px;
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
		padding-bottom: 20px;
		display: flex;
		border-bottom: 1px solid #000;
	}
	.articles-container h3 {
		margin: 20px 0;
		font-size: 2rem;
		text-transform: capitalize;
		font-weight: 400;
		border-bottom: 1.3px solid #f00;
	}
	.left {
		margin: 0 20px;
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.middle {
		flex: 2;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.right {
		margin: 0 20px;
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.todays-article-wrapper {
		width: 100%;
		max-width: 1024px;
		margin: 0 auto;
	}
	.todays-article-wrapper .heading-wrapper {
		width: 100%;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.todays-article-wrapper h3 {
		text-align: center;
		margin: 40px 0 20px 0;
		font-size: 3rem;
		border-bottom: 1px solid #f00;
	}


	@media (max-width: 1439px) {
		/* Laptop L */
	}
	@media (max-width: 1023px) {
		/* Laptop */
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
	@media (max-width: 767px) {
		/* Tablet */

		.todays-article-wrapper h3 {
			font-size: 2.5rem;
		}
	}
	@media (max-width: 424px) {
		/* Mobile L */
		.todays-article-wrapper h3 {
			font-size: 1.8rem;
		}
	}
	@media (max-width: 374px) {
		/* Mobile M */
	}
	@media (max-width: 319px) {
		/* Mobile S */
	}
</style>
