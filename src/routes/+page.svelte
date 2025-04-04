<script lang="ts">
</script>

<svelte:head>
	<title>Svelte Starter - Home</title>
	<meta name="description" content="Home page of the Svelte starter." />
</svelte:head>

<section>
	<h1 class="heading">Welcome to the Svelte starter</h1>
	<p class="presentation">
		This project aim to provide a satisfying starting point for any new project using Svelte kit.
	</p>

	<div class="features">
		<h2>Features</h2>
		<ul>
			<li>Color scheme</li>
			<li>Fluid sizing for fonts</li>
		</ul>
	</div>
</section>

<style lang="scss">
	section {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		flex: 0.6;

		.heading {
			width: 100%;
			text-align: center;
			margin-block-end: 3rem;
		}

		.presentation {
			width: 100%;
			text-align: center;
			margin-block-end: 3rem;
		}

		.features {
			width: 100%;
			padding: 1rem;
			background-color: var(--color-surface);
			box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
		}
	}
</style>
