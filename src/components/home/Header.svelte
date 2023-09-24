<header>
	<div>
		<img src="logos/normandie.png" alt="" />
		<img src="logos/greta.png" alt="" />
	</div>
	<nav>
		<ul>
			<li><a href="" class="primary-card">Programme</a></li>
			<li><a href="" class="primary-card">Exposants</a></li>
			<li><a href="" class="primary-card">Employeurs</a></li>
		</ul>
	</nav>
</header>

<style lang="scss">
	header {
		margin: 1em;
		display: flex;
		justify-content: space-between;
		align-items: center;
		div {
			display: flex;
			gap: 1em;
			img {
				height: 100px;
				@media screen and (max-width: 768px) {
					height: 50px;
				}
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
	}
</style>
