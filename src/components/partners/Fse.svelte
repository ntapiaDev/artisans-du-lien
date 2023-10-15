<div class="card">
	<div class="title">
		<h3>Fond Social Européen (FSE)</h3>
	</div>
	<div class="content">
		<img src="partners/fse.png" alt="Pole emploi" class="logo"/>
		<p>Le Fond Social Européen (FSE) participe à la mise en œuvre des politiques publiques nationales pour agir en faveur de l’emploi.</p>
		<p>Géré au niveau national, il a une portée d’actions et de solutions au cœur des territoires. Découvrez comment se traduit concrètement l’intervention de l’État en région Normandie. <p>L’objectif premier du FSE est de soutenir la création d’emplois de meilleure qualité dans l’UE et d’améliorer les perspectives professionnelles des citoyens (jeunes, demandeurs d’emploi, inactifs, handicapés, salariés étudiants etc.), prioritairement en direction des groupes les moins qualifiées et les plus exposés au chômage et à l’exclusion.</p>
		<p>En Normandie, si les disparités de niveau de vie entre territoires sont moins marquées que dans d’autres régions, il existe de fortes disparités selon les territoires et la typologie des habitants.</p>
		<p>Les jeunes, qui connaissent davantage de difficultés d’insertion, les actifs impactés par les mutations économiques et les femmes sont particulièrement exposés au chômage et à la pauvreté.</p>
		<a href="https://fse.gouv.fr" target="_blank">
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
