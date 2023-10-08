<script>
	let isBurgerOpen = false;
	// const toggleBurger = () => (isBurgerOpen = !isBurgerOpen);
</script>

<header>
	<a href="/"><img src="logos/greta.png" alt="" /></a>
	<nav>
		<ul>
			<li><a href="programme.pdf" class="primary-card">Programme</a></li>
			<li><a href="exposants" class="primary-card">Exposants</a></li>
			<li><a href="partenaires" class="primary-card">Partenaires</a></li>
		</ul>
	</nav>
	<!-- svelte-ignore a11y-click-events-have-key-events -->
	<!-- svelte-ignore a11y-no-static-element-interactions -->
	<!-- <div class="burger" on:click={toggleBurger}>
		<div class={'line' + (isBurgerOpen ? ' line1-active' : '')} />
		<div class={'line' + (isBurgerOpen ? ' line2-active' : '')} />
		<div class={'line' + (isBurgerOpen ? ' line3-active' : '')} />
	</div> -->
</header>

<style lang="scss">
	header {
		margin: 1em;
		display: flex;
		justify-content: space-between;
		align-items: center;
		img {
			height: 100px;
			@media screen and (max-width: 768px) {
				height: 75px;
			}
		}

		nav {
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

		// .burger {
		// 	width: 30px;
		// 	height: 20px;
		// 	display: flex;
		// 	flex-direction: column;
		// 	justify-content: space-between;
		// 	cursor: pointer;

		// 	@media screen and (min-width: 768px) {
		// 		display: none;
		// 	}

		// 	.line {
		// 		width: 30px;
		// 		height: 4px;
		// 		background-color: var(--primary-color);
		// 		transition: all 0.3s ease;
		// 	}

		// 	.line1-active,
		// 	.line2-active,
		// 	.line3-active {
		// 		background-color: var(--secondary-color);
		// 	}

		// 	.line1-active {
		// 		transform: translateY(8px) rotate(45deg);
		// 	}

		// 	.line2-active {
		// 		opacity: 0;
		// 		transform: translateX(-100vw);
		// 	}

		// 	.line3-active {
		// 		transform: translateY(-8px) rotate(-45deg);
		// 	}
		// }
	}
</style>
