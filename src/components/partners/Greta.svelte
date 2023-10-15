<div class="card">
	<div class="title">
		<h3>Le Réseau GRETA NORMANDIE</h3>
	</div>
	<div class="container">
		<div>
			<div class="content">
				<img src="logos/greta.png" alt="Greta Rouen Maritime" />
				<p>LES GRETA, Groupements d’établissements, sont les organismes de l’Éducation nationale qui assurent la mission de formation professionnelle continue.</p>
				<p>Demandeur.euse d’emploi, salarié.ée, entrepreneur.euse, individuel.elle,  le réseau régional des 3 GRETA de Normandie vous accueille sur tout le territoire normand pour vous apporter une réponse de proximité à vos besoins de formation en vous proposant :</p>
				<ul>
					<li>Une offre de pré-qualification</li>
					<li>Une offre d’orientation, conseil, bilan de compétences</li>
					<li>Une offre de formation ouverte sur tous les secteurs d’emploi (sanitaire/ social/ industrie/ tertiaire/ hôtellerie restauration/ environnement / hygiène / BTP)</li>
				</ul>
				<p>Ouvert à tous les publics, le réseau des GRETA privilégie une approche personnalisée et individualisée de la formation, chaque personne est accueillie et informée avant d’engager un parcours personnalisé dans le GRETA selon vos objectifs.
				Chaque GRETA normand est labellisé Eduform et certifié Qualiopi pour les actions de formation, les bilans de compétences et les actions permettant la validation des acquis de l’expérience (VAE).</p>
				<h4>LE GRETA ROUEN MARITIME :</h4>
				<p>Le GRETA Rouen Maritime dispense des formations pour les jeunes et adultes  en alternance en contrat d’apprentissage ou de professionnalisation.</p>
				<p>Nous formons également les personnes demandeurs d’emploi dans le cadre de formation financées par le Conseil Régional Normandie et le Pôle Emploi.</p>
				<p>Les salariés peuvent également bénéficier de formation dans le cadre du CPF, CPF de Transition ou ProA.</p>
				<p>Vous voulez préparer un diplôme, apprendre un métier, professionnaliser vos acquis, développer vos compétences et bénéficier d’une formation sur-mesure,  nous pouvons vous accompagner !</p>
				<p>Le Greta Rouen Maritime c’est 9 antennes de formation, plus de 20000 m² de salles et de bureaux, des équipements informatiques complets avec réseau pédagogique, 9 Espaces Atelier Insertion Remédiation, 1 Centre de Bilans de Compétences et d’accompagnement VAE avec trois lieux habilités.</p>
				<p>Tous secteurs d’activités représentés, un modèle pédagogique sur mesure avec possibilité de valider un ou des blocs de compétences pour toutes nos certifications.</p>
				Lien : <a href="https://greta.ac-normandie.fr/greta/greta-rouen-maritime" target="_blank">https://greta.ac-normandie.fr/greta/greta-rouen-maritime</a>
				<h4>Le GRETA PORTES NORMANDES :</h4>
				<p>Nos structures, nos ressources et notre connaissance du marché de l’emploi nous permettent de développer pour vous des formations multimodales, des parcours individualisés adaptés à vos besoins et contraintes, afin d’optimiser vos chances d’évolution et d’intégration professionnelles, via : </p>
				<ul>
					<li>12 antennes réparties sur le Calvados, l’Orne, l’Eure, et la Seine Maritime pour être au plus près de chez vous</li>
					<li>un savoir-faire démontré depuis 1975</li>
					<li>des collaborateurs expérimentés, professionnels de terrain et pédagogues avant tout</li>
					<li>des plateaux techniques performants dans ses domaines tels que la chaudronnerie, l’électricité, l’automobile, la chimie, la logistique, le service à la personne, le commerce...</li>
					<li>une relation forte avec les partenaires entreprises et institutionnels</li>
					<li>une veille permanente sur les métiers de demain</li>
				</ul>
				Lien : <a href="https://greta.ac-normandie.fr/greta/greta-portes-normandes" target="_blank">https://greta.ac-normandie.fr/greta/greta-portes-normandes</a>
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

				ul {
					padding-left: 2em;
				}

				h4 {
					margin: 1em 0;
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
