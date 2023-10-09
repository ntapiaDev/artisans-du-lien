<div class="atrium">
	<img src="photos/atrium.png" alt="" />
	<div class="container">
		<h3 class="primary-card">L'Atrium</h3>
		<div class="flex">
			<div class="infos">
				<div>115 Boulevard de l'Europe - 76100 ROUEN</div>
				<div><u>Pour tout renseignement :</u></div>
				<div>Greta Rouen Maritime - Antenne de Grand Quevilly</div>
				<div>02.32.11.01.06</div>
			</div>
			<div class="links">
				<a href="https://docs.google.com/forms/d/e/1FAIpQLSdhgABC-u2llTKw2tGmVNhLKAso-tlce2iHSuAFMt9_V6MG2w/viewform?usp=sf_link" target="_blank" class="primary-card">Inscription individuelle</a>
				<a href="https://docs.google.com/forms/d/e/1FAIpQLSdJpLDOBJmzjWS8IVYRQb3QLHK2QVI4mbO16bUOuAhM5Wa9Hw/viewform?usp=sf_link" target="_blank" class="primary-card">Inscription pour les groupes obligatoires</a>
			</div>
		</div>
	</div>
</div>

<style lang="scss">
	.atrium {
		margin-top: 1em;
		background-color: var(--background-color);
		position: relative;
		display: flex;
		gap: 1em;
		@media screen and (max-width: 1024px) {
			flex-direction: column;
			gap: 0;
		}

		img {
			width: 300px;
			@media screen and (max-width: 1024px) {
				width: 100%;
			}
		}

		.container {
			padding: 1em;
			flex-grow: 1;
			flex-direction: column;
			gap: 0;

			h3 {
				padding-left: 1em;
				font-size: 3em;
			}

			.flex {
				margin-top: 1em;
				padding: 1em;
				display: flex;
				justify-content: space-between;

				@media screen and (max-width: 1024px) {
					margin-top: 0;
					flex-direction: column;
					gap: 1em;
				}

				.infos,
				.links {
					display: flex;
					flex-direction: column;
					gap: 0.5em;
					color: var(--secondary-color);
					font-size: 1.25em;

					a {
						padding: 0.5em;
					}

					@media screen and (max-width: 1024px) {
						margin-top: 0.5em;
					}
				}
			}
		}
	}
</style>
