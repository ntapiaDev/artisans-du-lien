<div class="container">
	<div class="date primary-card">
		<div>Le lundi</div>
		<div>novembre de</div>
		<div>9h30 à 16h30</div>
		<div class="digit secondary-card">13</div>
	</div>
	<h3 class="primary-card">Le salon</h3>
	<p>Relier les acteurs de l’accompagnement au service du maintien à domicile pour en donner une vision différente, actualisée, c’est là l’idée principale de cet événement.</p>
	<img src="icons/meeting.png" alt="Meeting" class="meeting">
	<p>Geste, parole, outil, matériel ou équipement, nous cherchons à donner à voir et à partager les expériences et les innovations qui traduisent l’importance de cet accompagnement humain au cœur de nos activités.</p>
	<img src="icons/tablet.png" alt="Tablet" class="tablet">
	<p>Cet accompagnement se tisse au quotidien, s’ajuste au plus près des personnes et de leurs besoins, il se façonne techniquement et relationnellement. C’est la raison pour laquelle nous avons donc choisi de nommer cet événement « Artisans du lien ».</p>	
	<p>Nos valeurs portées sur la bienveillance nous ont amenés à choisir la date du 13 novembre, journée dédiée à cette approche.</p>
	<p>Que vous soyez professionnel, en cours ou en devenir, en découverte, aidant, bénéficiaire, nous vous invitons à sillonner autour des ateliers, à échanger, expérimenter... découvrez le domaine du maintien à domicile autrement !!</p>
	<p>Et si au détour de cette expérience, nous avons réussi à changer votre regard, votre perception de ce domaine, à vous faire connaitre une technique, un outil, un dispositif, vous aider à élargir votre réseau, à trouver un emploi, une formation... alors notre objectif sera atteint.</p>
</div>

<style lang="scss">
	.container {
		margin: 1em 0 2em;
		padding: 0 1em;
		text-align: justify;
		@media screen and (max-width: 768px) {
			display: flex;
			flex-direction: column;
		}

		.date {
			float: right;
			min-width: 350px;
			margin-right: 90px;
			margin-left: 1em;
			padding-left: 1em;
			height: 150px;
			font-size: 2em;
			position: relative;
			@media screen and (max-width: 768px) {
				min-width: 0;
				margin-top: 1em;
				margin-left: 0;
				height: 110px;
				font-size: 1.5em;
				order: 1;
			}
			.digit {
				width: 180px;
				height: 180px;
				position: absolute;
				top: -15px;
				right: -90px;
				border-radius: 50%;
				font-size: 4em;
				font-style: normal;
				font-weight: bold;
				display: flex;
				justify-content: center;
				align-items: center;
				@media screen and (max-width: 768px) {
					width: 125px;
					height: 125px;
					top: -8px;
					font-size: 4.2em;
				}
			}
		}

		h3 {
			margin-bottom: 0.5em;
			padding-left: 1em;
			font-size: 2em;
			display: flex;
		}

		p {
			margin-left: 0.5em;
			color: var(--secondary-color);
			font-size: 1.5em;

			& + p {
				margin-top: 0.5em;
			}

			@media screen and (max-width: 768px) {
				margin-left: 0;
				font-size: 1.25em;
			}
		}

		img {
			width: 200px;

			&.meeting {
				float: left;
				margin: 1em 1em 1em 0;
			}

			&.tablet {
				float: right;
				margin: 1em 0 1em 1em;
			}

			&.meeting,
			&.tablet {
				@media screen and (max-width: 768px) {
					width: calc(100% - 2em);
					margin: 1em;
				}
			}
		}
	}
</style>
