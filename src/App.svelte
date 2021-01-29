<script>
	import Header from './Header.svelte'
	import Article from './Article.svelte'
</script>

<div class="container">
	<Header />
	<main>
		<Article />
		<Article />
		<Article />
		<Article />
		<Article />
		<Article />
		<Article />
		<Article />
	</main>
</div>

<style>

	.container {
		min-width: 600px;
		width: 1000px;
		/* background-color: rgb(241, 247, 252) */
		margin: 0 auto;
	}

</style>