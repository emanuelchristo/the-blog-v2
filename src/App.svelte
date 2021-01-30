<script>
	import Header from "./Header.svelte";
	import Article from "./Article.svelte";
	import ArticleCard from "./ArticleCard.svelte"
</script>

<div class="container">
	<div class="header-wrapper">
		<Header />
	</div>

	<main>
		<div class="article-wrapper">
			<Article index="1" />
			<Article index="2" />
		</div>
		
		<div class="article-card-wrapper">
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
			<ArticleCard />
		</div>

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

	.header-wrapper {
		position: fixed;
		margin: 0 auto;
		width: 100%;
		min-width: 300px;
		max-width: 1300px;
		left: 0;
		right: 0;
		top: 0;
	}

	main {
		margin-top: 12rem;
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
</style>
