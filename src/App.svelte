<script>
	import Header from "./Header.svelte";
	import Article from "./Article.svelte";
</script>

<div class="container">
	<div class="header-wrapper">
		<Header />
	</div>

	<main>
		<Article index="1" />
		<Article index="2" />
		<Article index="3" />
		<Article index="4" />
		<Article index="5" />
		<Article index="6" />
		<Article index="7" />
		<Article index="8" />
		<Article index="9" />
	</main>
</div>

<style>
	.container {
		min-width: 600px;
		width: 1000px;
		/* background-color: rgb(241, 247, 252) */
		margin: 0 auto;
		position: relative;
	}

	.header-wrapper {
		position: fixed;
		margin: 0 auto;
		width: 1000px;
		min-width: 600px;
		left: 0;
		right: 0;
		top: 0;
	}

	main {
		margin-top: 12rem;
	}
</style>
