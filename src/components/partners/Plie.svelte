<div class="card">
	<div class="title">
		<h3>PLIE METROPOLE ROUEN</h3>
	</div>
	<div class="content">
		<img src="partners/plie.png" alt="Pole emploi" class="logo"/>
		<p>Depuis 1997, la Métropole Rouen Normandie s’est engagée aux côtés de l’Etat, de la Région Normandie et du Département de Seine Maritime dans la mise en œuvre d’un Plan Local pour l’Insertion et l’Emploi (PLIE).</p>
		<p>Ce dispositif a pour objectif l'accès à l'emploi des femmes et des hommes confronté.e.s à une exclusion du marché du travail. Pour y parvenir il propose des parcours d'insertion individualisés prenant en considération l'ensemble des besoins des personnes. Chacune est soutenue dans ses démarches par un.e référent.e appelé.e «Accompagnat.eur.rice Emploi».</p>
		<p>Chaque demandeur.euse d’emploi accompagné.e devient « adhérent.e » du PLIE et bénéficie de l’appui permanent d’une personne ressource dès son entrée dans le PLIE. Le rythme des rencontres est adapté à sa situation et à l’évolution de son parcours.</p>
		<p>Cet Accompagnateur.rice emploi propose et met en place un parcours d’insertion professionnelle personnalisé sans limitation de durée, prenant en compte l’ensemble des besoins de la personne. Ce parcours est composé de diverses étapes dont le choix est déterminé avec l’adhérent.e, il peut s’agir d’actions d’orientation, d’évaluation, de formation, de soutien à la recherche d’emploi, de mises en situations de travail…</p>
		<p>Toutes ces étapes sont suivies par l’accompagnateur.rice emploi afin d’en mesurer les effets et d’ajuster le parcours si nécessaire.</p>
		<p>Le suivi se poursuit jusqu’aux 6 premiers mois de l’emploi obtenu à l’issue de ce parcours ou aux 6 mois suivants l’obtention d’un diplôme.</p>
		<p>Cet accompagnement est réalisé par les acteurs du PLIE de la Métropole Rouen ou par des prestataires de la mission, au sein des structures de l’ADEP, la Mission Locale, Education et formation, Inseraction.</p>
		<a href="https://www.pliedelametropole.fr/orienter-et-accompagner/trouver-un-accompagnateur-emploi" target="_blank">
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

				@media screen and (max-width: 768px) {
					width: 100%;
				}

				img {
					width: 30px;
					height: 30px;
				}
			}
		}
	}
</style>
