<div class="card">
	<div class="title">
		<h3>L’Atrium</h3>
	</div>
	<div class="content">
		<img src="partners/atrium.png" alt="Pole emploi" class="logo"/>
		<p>Au cœur de la cité rouennaise, l’Atrium est un espace à destination de tous et notamment des jeunes normands, pour une meilleure appropriation du savoir et plus largement de leur environnement régional en matière d’orientation et de découverte des métiers.</p>
		<p>Riche de cette histoire, l’Atrium est aujourd’hui l’espace régional de découverte scientifique technique et industriel en Normandie.</p>
		<p>L’Atrium est le fruit d’un partenariat unique en France entre une association de culture scientifique, Science Action Normandie, et l’Agence régionale de l’orientation et des métiers de Normandie.</p>
		<p>C’est aussi une offre originale autour d’un triptyque identitaire fort qui façonne les différents espaces d’exposition sur :</p>
		<ul>
			<li>Les sciences et la valorisation de ce secteur auprès de tous les publics.</li>
			<li>L’orientation à travers l’espace « Orientation et métiers » en partenariat avec l’Agence régionale de l’Orientation et des Métiers de Normandie.</li>
			<li>Les métiers et les savoir-faire des filières d’excellence normandes.</li>
		</ul>
		<a href="https://www.atriumnormandie.fr" target="_blank">
			<img src="icons/website_p.png" alt="site internet" />Site internet
		</a>
	</div>
	<img class="atrium" src="photos/atrium.webp" alt="L'atrium">
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

			ul {
				padding-left: 2em;
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

		.atrium {
			width: calc(100% - 2em);
			margin: 0 1em 1em;
			border-radius: 1em;
		}
	}
</style>
