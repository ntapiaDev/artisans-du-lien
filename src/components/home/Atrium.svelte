<div>
	<img src="photos/atrium.png" alt="" />
	<div>
		<h3 class="primary-card">L'Atrium</h3>
		<div>115 Boulevard de l'Europe - 76100 ROUEN</div>
		<div>Pour tout renseignement : 02.32.11.01.06</div>
		<div>(GRETA de GRAND-QUEVILLY)</div>
	</div>
	<img src="icons/atrium.png" alt="" class="background" />
</div>

<style lang="scss">
	div {
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

        div {
			padding: 1em;
            flex-grow: 1;
            flex-direction: column;
            gap: 0;

            h3 {
				padding-left: 1em;
                font-size: 3em;
            }

			div {
				padding: 0;
				flex-grow: 0;
			}
        }

		.background {
			position: absolute;
			right: 0;
			bottom: 0;
            @media screen and (max-width: 1024px) {
                width: 100px;
            }
		}
	}
</style>
