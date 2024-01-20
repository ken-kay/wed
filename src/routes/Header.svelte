<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
</script>

<header>
	
	<nav class="fixed right-0 left-0">
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z" />
		</svg>
		<ul class="gap-4">
			<li class="hover:text-blue-500"
				aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="#accommodation">Accommodation</a>
			</li>
			<li class="hover:text-blue-500"
				aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="#directions">Directions</a>
			</li>
			<li class="hover:text-blue-500"
				aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="#gifts">Gifts</a>
			</li>

			<!-- <li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">About</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/sverdle') ? 'page' : undefined}>
				<a href="/sverdle">Sverdle</a>
			</li> -->

		</ul>
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z" />
		</svg>
	</nav>

	<div class="corner fixed left-0 hover:bg-blue-200 rounded-full hidden md:block">
		<a href="/">
			<img class="hover:scale-110 " 
				src="./favicon.png" alt="logo" />
		</a>
	</div>
	


	<div class="corner fixed right-0 rounded-full hidden md:block">
		<a href="https://justrsvp.me/moww" target="_blank">
			<p class="z-20 fixed font-semibold hover:scale-110 hover:text-blue-500">RSVP</p>
			<img class="hover:scale-110 " 
				src="./white.png" alt="rsvp" />
		</a>
		

	</div>

	<!-- -->
		
</header>

	<div class="w-full bg-center bg-cover h-[100vh]" 
			style="background-image: url('./top.jpg');"			
			>
			<div class="flex items-center justify-center w-full bg-white bg-opacity-70 h-full "> <!-- bg-gray-900/40 -->
				<div class="text-center">
					<!-- <h1 class="text-3xl font-semibold text-white lg:text-4xl">Build your new <span class="text-blue-400">Saas</span> Project</h1>
					<button class="w-full px-5 py-2 mt-4 text-sm font-medium text-white capitalize transition-colors duration-300 transform bg-blue-600 rounded-md lg:w-auto hover:bg-blue-500 focus:outline-none focus:bg-blue-500">Start project</button> -->
					<h1 class="font-['Style_Script'] text-6xl font-extrabold">
						Marion Orina
					</h1>
					<h1 class="font-['Style_Script'] text-6xl font-extrabold">
						&
					</h1>
					<h1 class="font-['Style_Script'] text-6xl mb-4 font-extrabold">
						Wachira Waigwa
					</h1>
					<p class="mb-8 leading-relaxed text-4xl font-semibold">
						Friday March 1<sup>st</sup>, 2024
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
		--background: rgba(255, 255, 255, 0.7);
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
