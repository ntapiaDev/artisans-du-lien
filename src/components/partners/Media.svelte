<div class="card">
	<div class="title">
		<h3>Media Formation</h3>
	</div>
	<div class="content">
		<img src="partners/media.png" alt="Media Formation" class="logo"/>
		<p>Média Formation est un organisme de formation, sous statut associatif.</p>
		<p>Nos missions sont avant tout de favoriser l’insertion, faciliter l’accès, le maintien ou la promotion en emploi.</p>
		<p>Un Pôle est dédié à l’accompagnement des personnes, salariées ou non, souhaitant découvrir, ou se former et se qualifier dans les Services et l’Aide à la Personne.</p>
		<a href="https://www.media-formation.fr" target="_blank">
			<img src="icons/website_p.png" alt="site internet" />Site internet
		</a>
	</div>
</div>

<style lang="scss">
	.card {
		background-color: var(--background-color);
		border-radius: 1em;
		display: flex;
		flex-direction: column;

		@media screen and (max-width: 768px) {
			margin-top: 1em;
		}

		.title {
			background-color: var(--primary-color);
			border-radius: 1em;
			padding: 0.5em 1em;
			display: flex;
			justify-content: space-between;
			align-items: center;
			gap: 1em;

			@media screen and (max-width: 768px) {
				flex-direction: column;
				gap: 0.5em;
			}

			h3 {
				font-size: 2em;
				text-transform: uppercase;
				color: var(--secondary-color);
				text-align: center;

				@media screen and (max-width: 768px) {
					font-size: 1.5em;
				}
			}
		}

		.content {
			padding: 1em;
			text-align: justify;

			.logo {
				float: left;
				margin: 0 1em 0 0;
				max-width: 200px;
				max-height: 100px;
			}

			p + p {
				margin-top: 1em;
			}

			a {
				width: 151px;
				margin-left: auto;
				margin-top: 1em;
				padding: 0.5em 1em;
				color: #ffffff;
				background-color: var(--primary-color);
				border-radius: 2em;
				display: flex;
				align-items: center;
				justify-content: center;
				gap: 1em;

				img {
					width: 30px;
					height: 30px;
				}
			}
		}
	}
</style>
