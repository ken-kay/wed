<script>
	import { page } from '$app/stores';
</script>

<header class="">
	<nav class="fixed right-0 left-0">
		<ul class="gap-4 w-full">
			<li class=" hover:text-blue-500 hover:scale-110"
				aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="#accommodation">Accommodation</a>
			</li>
			<li class="hover:text-blue-500 hover:scale-110"
				aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="#directions">Directions</a>
			</li>
			<li class="hover:text-blue-500 hover:scale-110"
				aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="#gifts">Gifts</a>
			</li>
		</ul>
	</nav>

	<div class="corner fixed left-0 hover:bg-blue-200 rounded-full hidden md:block">
		<a href="/">
			<img class="hover:scale-110 " 
				src="./favicon.png" alt="logo" />
		</a>
	</div>
	


	<div class="corner fixed right-0 rounded-full hidden md:block">
		<a href="/">
			<p class="z-20 fixed font-semibold hover:scale-110 hover:text-blue-500">RSVP</p>
			<img class="hover:scale-110 " 
				src="./white.png" alt="rsvp" />
		</a>
	</div>
		
</header>

	<div class="w-full bg-center bg-cover h-[100vh]" 
			style="background-image: url('./top.jpg');"			
			>
			<div class="flex items-center justify-center w-full bg-white bg-opacity-70 h-full ">
				<div class="text-center">
					<h1 class="font-['Style_Script'] text-6xl font-extrabold">
						Mademoiselle
					</h1>
					<h1 class="font-['Style_Script'] text-6xl font-extrabold">
						&
					</h1>
					<h1 class="font-['Style_Script'] text-6xl mb-4 font-extrabold">
						Monsieur
					</h1>
					<p class="mb-8 leading-relaxed text-4xl font-semibold">
						Thursday February 29<sup>th</sup>, 2024
					</p>
				</div>
			</div>
		</div>

<style>
	header {
		display: flex;
		justify-content: space-between;
	}

	.corner {
		width: 3em;
		height: 3em;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	.corner img {
		width: 2em;
		height: 2em;
		object-fit: contain;
	}

	nav {
		display: flex;
		justify-content: center;
		--background: rgba(165, 228, 253, 0.336);
	}

	svg {
		width: 2em;
		height: 3em;
		display: block;
	}

	path {
		fill: var(--background);
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page']::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-1);
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-1);
	}
</style>
