<div class="container">
	<div class="title">
		<h3 class="primary-card">Le salon</h3>
		<p>Venez participer aux ateliers, rencontrer des professionnels et découvrir des outils et dispositifs innovants pour accompagner à domicile.</p>
	</div>
	<div class="date primary-card">
		<div>Le vendredi</div>
		<div>novembre</div>
		<div>de 10h à 16h</div>
		<div class="digit secondary-card">13</div>
	</div>
</div>

<style lang="scss">
	.container {
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
				@media screen and (max-width: 768px) {
					font-size: 3em;
				}
			}
			p {
				margin-top: 1em;
				color: var(--secondary-color);
				@media screen and (max-width: 768px) {
					font-size: 2em;
				}
			}
		}

		.date {
			margin-right: 90px;
			padding-left: 1em;
			padding-right: calc(1em + 90px);
			height: 150px;
			font-size: 2em;
			position: relative;
			@media screen and (max-width: 768px) {
				height: 100px;
				font-size: 2.8em;
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
					width: 120px;
					height: 120px;
					top: -10px;
					font-size: 4.2em;
				}
			}
		}
	}
</style>
