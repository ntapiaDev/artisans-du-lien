<div class="card">
	<div class="title">
		<h3>Pole emploi</h3>
	</div>
	<div class="content">
		<img src="partners/pe.svg" alt="Pole emploi" class="logo"/>
		<p>Pôle emploi est le service public de l’emploi en France. Son rôle est, d’une part, d’indemniser les demandeurs d’emploi et les accompagner vers le retour à l’emploi ; et d’autre part, de guider les entreprises dans leurs recrutements.</p>
		<h4>Au service des demandeurs d’emplois :</h4>
		<p>Pôle emploi gère les dossiers d’indemnisations selon les droits des salariés en rupture ou fin de contrat. Il propose sur l’ensemble de ses antennes des services d’orientation aussi bien généralistes que spécialisés, avec des prestations adaptées aux profils et aux besoins de formation de tous les publics, tout au long de la vie. Aux côtés des Conseils régionaux, le Pole Emploi compte ainsi parmi les principaux financeurs de formations pour les demandeurs d’emploi. Un rôle essentiel en matière de prescription et un levier majeur d’accès à l’emploi.</p>
		<p>Il permet d'accéder aux services de recherche d'emploi (diffusion de votre CV, abonnement aux offres publiées, ...) et, si vous êtes inscrit à Pôle emploi, aux informations et services sur vos allocations</p>
		<a href="https://www.emploi-store.fr/portail/accueil" target="_blank">
			<img src="icons/website_p.png" alt="site internet" />Site internet
		</a>
		<h4>Au service des entreprises :</h4>
		<p>Grâce à leur espace dédié sur pole-emploi.fr, les employeurs peuvent gérer directement leurs besoins de recrutement : déposer leurs offres, présenter leur activité et contacter les demandeurs d’emploi répondant aux profils qu’ils recherchent.</p>
		<p>En complément, Pôle emploi propose des services d’accompagnement sur mesure et d’appui aux employeurs ayant des difficultés à recruter ou à définir leurs besoins. Dans le cadre de ces services particulièrement adaptés, par exemple, aux entreprises de petite taille ou placées sur des métiers de niche, les conseillers de Pôle emploi peuvent procéder à des analyses de poste, fournir un support aux entretiens d’embauche, présélectionner des candidatures, ou bien encore conduire des actions d’adaptation des demandeurs d’emploi aux postes de travail proposés.</p>
		<a href="https://www.pole-emploi.fr/region/normandie" target="_blank">
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

			h4 {
				margin: 1em 0;
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
