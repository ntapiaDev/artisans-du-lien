<div class="card">
	<div class="title">
		<h3>Le Conseil Départemental Seine-Maritime</h3>
	</div>
	<div class="content">
		<img src="partners/76.png" alt="Pole emploi" class="logo"/>
		<p>Chef de file de l’action sociale, Le département Seine Maritime prend en charge l’aide sociale, l’autonomie des personnes, l’insertion et l’emploi et la promotion des solidarités.  </p>
		<p>Le Conseil départemental agit avec tous les acteurs du territoire, pour le bien-être et l’autonomie des personnes âgées et handicapées. L’objectif principal est de préserver ou d’améliorer la qualité de vie et de maintenir ou favoriser l’autonomie à travers de nombreuses aides et dispositifs, dont (entre autres) :</p>
		<ul>
			<li>l’Allocation personnalisée d’autonomie (APA)</li>
			<li>la prestation de compensation du handicap (PCH)</li>
			<li>la Maison Départementale des Personnes Handicapées, structure d’accueil et d’accompagnement pour les personnes handicapées, leur famille mais aussi pour les soignants, professionnels et services du Département</li>
		</ul>
		<h4>CLIC (Centres Locaux d'Information et de Coordination)</h4>
		<p>En Seine-Maritime, le Département délègue sa compétence de coordination gérontologique aux CLIC.</p>
		<p>La totalité du territoire départemental est couvert par 16 CLIC qui exercent des missions en faveur des personnes âgées de 60 ans et plus, de leurs proches aidants et également des professionnels du secteur gérontologique.</p>
		<p>Ainsi, en soutien des acteurs locaux de premiers recours, ces centres exercent une mission d’accueil, d’information et d’orientation du public âgé de 60 ans et plus mais également de ses proches.</p>
		<p>L’équipe du CLIC se déplace au domicile de la personne afin de lui proposer une évaluation multidimensionnelle de ses besoins et un plan d’accompagnement dont elle assure le suivi.</p>
		<!-- <a href="" target="_blank">
			<img src="icons/website_p.png" alt="site internet" />Site internet
		</a> -->
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

			p + p {
				margin-top: 1em;
			}

			ul {
				padding-left: 2em;
			}

			// a {
			// 	width: 151px;
			// 	margin-left: auto;
			// 	margin-top: 1em;
			// 	padding: 0.5em 1em;
			// 	color: #ffffff;
			// 	background-color: var(--primary-color);
			// 	border-radius: 2em;
			// 	display: flex;
			// 	align-items: center;
			// 	justify-content: center;
			// 	gap: 1em;

			// 	img {
			// 		width: 30px;
			// 		height: 30px;
			// 	}
			// }
		}
	}
</style>
