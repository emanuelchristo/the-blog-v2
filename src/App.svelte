<script>
	import Header from "./Header.svelte";
	import Article from "./Article.svelte";
	import ArticleCard from "./ArticleCard.svelte"
	import Article2 from "./Article2.svelte"
</script>

<div class="container">
	<div class="header-wrapper">
		<Header />
	</div>

	<main>
		<div class="articles-container">
			<div class="left">
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
			</div>
			<div class="middle">
				<Article2 />
				<Article2 />
				<Article2 />
				<Article2 />
			</div>
			<div class="right">
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
				<ArticleCard />
			</div>
		</div>

		<div class="article-wrapper">
			<Article index="1" />
			<Article index="2" />
			<Article index="3" />
			<Article index="4" />
			<Article index="5" />
			<Article index="6" />
			<Article index="7" />
		</div>
		
		<!--
		<div class="article-card-wrapper">
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
		</div> -->

	</main>
</div>

<style>
	.container {
		min-width: 300px;
		max-width: 1300px;
		width: 100%;
		/* background-color: rgb(241, 247, 252) */
		margin: 0 auto;
		position: relative;
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
	.article-wrapper {
		width: 80%;
		margin: 0 auto;
	}
	.article-card-wrapper {
		margin: 0 auto;
		width: 80%;
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		padding-bottom: 20rem;
		padding-top: 7rem;
	}

	.articles-container {
		display: flex;
		border-bottom: 1px solid #000;
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

	@media (max-width: 600px) {
		main {
			margin-top: 8rem;
		}
	}
</style>
