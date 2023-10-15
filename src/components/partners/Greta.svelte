<div class="card">
	<div class="title">
		<h3>GRETA ROUEN MARITIME</h3>
		<span>"Antenne de Grand Quevilly"</span>
	</div>
	<div class="container">
		<div>
			<div class="content">
				<img src="logos/greta.png" alt="Greta Rouen Maritime" />
				<p>Depuis plus de 50 ans, le GRETA Rouen Maritime dispense des formations pour les jeunes en alternance en contrat d’apprentissage et de professionnalisation.</p>
				<p>Nous formons également les personnes demandeurs d’emploi dans le cadre de formations financées par le Conseil Régional Normandie et le Pôle Emploi.</p>
				<p>Les salariés peuvent également bénéficier de formation dans le cadre du CPF, CPF de Transition ou ProA.</p>
				<p>Vous voulez préparer un diplôme, apprendre un métier, professionnaliser vos acquis, développer vos compétences et bénéficier d’une formation sur-mesure nous pouvons vous accompagner !</p>
				<p>Le Greta Rouen Maritime c’est 9 antennes de formation, plus de 20000 m² de salles et de bureaux, des équipements informatiques complets avec réseau pédagogique, 9 Espaces Atelier Insertion Remédiation, 1 Centre de Bilans de Compétences et d’accompagnement VAE avec trois lieux habilités.</p>
				<p>Tous secteurs d’activités représentés, un modèle pédagogique sur mesure avec possibilité de valider un ou des blocs de compétences pour toutes nos certifications.</p>
			</div>
			<div class="contact">
				<span></span>
				<span>
					<a href="https://greta.ac-normandie.fr/greta/greta-rouen-maritime" target="_blank">
						<span class="website">
							<img src="icons/website_p.png" alt="site internet" />Site internet
						</span>
					</a>
				</span>
			</div>
		</div>
		<iframe src="https://www.youtube.com/embed/gYWQyaWXltg" title="Vidéo de présentation du GRETA ROUEN MARITIME " frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
	</div>
</div>

<style lang="scss">
	.card {
		margin: 1em;
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
				white-space: nowrap;

				@media screen and (max-width: 768px) {
					font-size: 1.5em;
				}
			}

			span {
				font-size: 1.5em;
				color: #ffffff;
				text-align: end;

				@media screen and (max-width: 768px) {
					font-size: 1em;
					text-align: center;
				}
			}
		}

		.container {
			padding: 1em;
			display: flex;
			gap: 1em;

			@media screen and (max-width: 768px) {
				flex-direction: column;
			}

			&> div,
			iframe {
				width: 50%;
				@media screen and (max-width: 768px) {
					width: 100%;
				}
			}

			.content {
				text-align: justify;

				img {
					float: left;
					margin: 0 1em 0 0;
					max-width: 200px;
					max-height: 100px;
				}
			}

			.contact {
				margin-top: auto;
				display: flex;
				justify-content: space-between;

				@media screen and (max-width: 768px) {
					flex-direction: column;
					gap: 1em;
				}

				span {
					display: flex;
					gap: 1em;

					@media screen and (max-width: 768px) {
						width: 100%;
					}

					a {
						color: #ffffff;
						display: block;
						width: 100%;
					}

					.website {
						padding: 0.5em 1em;
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
		}
	}
</style>
