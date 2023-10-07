<div class="container">
	<div class="title">
		<h3 class="primary-card">Le salon</h3>
		<p>Venez participer aux ateliers, rencontrer des professionnels et découvrir des outils et dispositifs innovants pour accompagner à domicile.</p>
	</div>
	<div class="date primary-card">
		<div>Le lundi</div>
		<div>novembre de</div>
		<div>9h30 à 16h30</div>
		<div class="digit secondary-card">13</div>
	</div>
</div>

<style lang="scss">
	.container {
		margin: 1em 0 2em;
		padding: 0 1em;
		display: flex;
		gap: 1em;
		@media screen and (max-width: 768px) {
			flex-direction: column;
		}

		.title {
			flex-grow: 1;
			h3 {
				padding-left: 1em;
				font-size: 2em;
			}
			p {
				margin-top: 0.5em;
				margin-left: 0.5em;
				color: var(--secondary-color);
				font-size: 1.5em;
			}
		}

		.date {
			min-width: 350px;
			margin-right: 90px;
			padding-left: 1em;
			height: 150px;
			font-size: 2em;
			position: relative;
			@media screen and (max-width: 768px) {
				min-width: 0;
				height: 110px;
				font-size: 1.5em;
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
	}
</style>
