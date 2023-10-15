<div class="card">
	<div class="title">
		<h3>REGION NORMANDIE</h3>
	</div>
	<div class="content">
		<img src="partners/normandie.png" alt="Pole emploi" class="logo"/>
		<p>La Région Normandie est le chef de file de la politique régionale de formation et d’insertion professionnelles en direction des jeunes et des adultes : apprentis, chômeurs, travailleurs sociaux, professions paramédicales.</p>
		<p>A ce titre, elle finance des dispositifs permettant aux normands de s’orienter, se former, et trouver un emploi.</p>
		<p>Quel que soit votre statut (demandeur d’emploi, salarié, travailleur indépendant, artisan…), la Région Normandie vous accompagne tout au long de votre parcours dans votre projet professionnel, en synergie avec l’ensemble des acteurs de l’orientation, de l’emploi, de l’insertion professionnelle et de la formation.</p>
		<a href="https://parcours-metier.normandie.fr" target="_blank">
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
