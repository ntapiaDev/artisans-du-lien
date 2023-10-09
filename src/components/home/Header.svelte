<script>
	import { page } from '$app/stores';

	let isBurgerOpen = false;
	const toggleBurger = () => (isBurgerOpen = !isBurgerOpen);
</script>

<header>
	{#if $page.url.pathname === '/'}
		<a href="/"><img src="logos/greta.png" alt="" /></a>
	{:else}
		<a href="/" class="primary-card home">Accueil</a>
	{/if}
	<nav class="desktop-nav">
		<ul>
			<li><a href="programme.pdf" class="primary-card" target="_blank">Programme</a></li>
			<li><a href="exposants" class="primary-card">Exposants</a></li>
			<li><a href="partenaires" class="primary-card">Partenaires</a></li>
		</ul>
	</nav>
	<!-- svelte-ignore a11y-click-events-have-key-events -->
	<!-- svelte-ignore a11y-no-static-element-interactions -->
	<div class={'burger' + (isBurgerOpen ? ' active' : '')} on:click={toggleBurger}>
		<div class={'line' + (isBurgerOpen ? ' line1-active' : '')} />
		<div class={'line' + (isBurgerOpen ? ' line2-active' : '')} />
		<div class={'line' + (isBurgerOpen ? ' line3-active' : '')} />
	</div>
	<nav class={'mobile-nav' + (isBurgerOpen ? ' active' : '')}>
		<ul>
			<li><a href="/">Accueil</a></li>
			<li><a href="programme.pdf" target="_blank">Programme</a></li>
			<li><a href="exposants">Exposants</a></li>
			<li><a href="partenaires">Partenaires</a></li>
		</ul>
	</nav>
</header>

<style lang="scss">
	header {
		margin: 1em;
		display: flex;
		justify-content: space-between;
		align-items: center;
		position: relative;

		img {
			height: 100px;
			@media screen and (max-width: 768px) {
				height: 75px;
			}
		}

		.home {
			padding: 0.25em 1em;
			font-size: 1.5em;
			text-decoration: none;
		}

		.desktop-nav {
			@media screen and (max-width: 768px) {
				display: none;
			}
			ul {
				display: flex;
				gap: 1em;
				list-style: none;
				li a {
					padding: 0.25em 1em;
					font-size: 1.5em;
					text-decoration: none;
				}
			}
		}

		.mobile-nav {
			height: 0;
			overflow: hidden;
			position: absolute;
			top: -1em;
			left: -1em;
			width: calc(100% + 2em);
			background-color: var(--primary-color);
			box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.5);
			transition: all 0.3s ease;

			&.active {
				height: 176px;
			}

			ul {
				padding: 1em;
				list-style: none;
				li a {
					font-size: 1.5em;
					color: var(--secondary-color);
					text-decoration: none;
				}
			}
		}

		.burger {
			width: calc(30px + 1em);
			height: calc(20px + 1em);
			padding: 0.5em;
			background-color: var(--secondary-color);
			border-radius: 0.5em;
			display: flex;
			flex-direction: column;
			justify-content: space-between;
			z-index: 999;
			cursor: pointer;

			&.active {
				background-color: var(--primary-color);
			}

			@media screen and (min-width: 768px) {
				display: none;
			}

			.line {
				width: 30px;
				height: 4px;
				background-color: var(--primary-color);
				transition: all 0.3s ease;
			}

			.line1-active,
			.line2-active,
			.line3-active {
				background-color: var(--secondary-color);
			}

			.line1-active {
				transform: translateY(8px) rotate(45deg);
			}

			.line2-active {
				opacity: 0;
			}

			.line3-active {
				transform: translateY(-8px) rotate(-45deg);
			}
		}
	}
</style>
