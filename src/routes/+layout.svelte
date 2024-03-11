<script>
	import Header from './Header.svelte';
	import './styles.css';
	import "../app.css";
  import Accommodation from '../components/Accommodation.svelte';
//   import Directions from '../components/Directions.svelte';
  import Map from '../components/Map.svelte';
  import Gifts from '../components/Gifts.svelte';
</script>

<div class="app">
	<Header />
	<Accommodation/>
	<!-- <Directions /> -->
	<Map />
	<Gifts />

	<main>
		<slot />
	</main>

	<footer>
		<p class="text-md">Made by <a href="https://kenani.dev" class="text-blue-500 hover:text-green-500">Kenani</a> with care</p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	/* .title {
		display: flex;
		font-family: "Sofia", sans-serif;
	} */

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
