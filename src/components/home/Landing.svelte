<aside>
	<h1>
		<span>Les <img src="icons/icon1.png" alt="" /></span>
		<span>artisans</span>
		<span>du lien <img src="icons/house.png" alt="" /></span>
	</h1>
	<div class="primary-card">Chez vous au quotidien</div>
	<h2>Redécouvrez l'aide à domicile</h2>
</aside>

<style lang="scss">
	aside {
		margin: 1em;
		display: inline-flex;
		flex-direction: column;

		h1,
		h2 {
			color: #ffffff;
			font-family: 'Open Sans', sans-serif;
		}

		h1 {
			font-size: 6em;
			text-transform: uppercase;
			display: inline-flex;
			flex-direction: column;

			span:nth-child(1) {
				display: flex;
				justify-content: space-between;
				align-items: baseline;
				img {
					width: 150px;
				}
			}

			span:nth-child(3) {
				display: flex;
				align-items: flex-end;
				img {
					margin-left: 1em;
					width: 150px;
					@media screen and (max-width: 1024px) {
						width: 100px;
					}
				}
			}
		}

		div {
			font-size: 3.8em;
		}

		h2 {
			margin-top: 0.5em;
			font-size: 2.5em;
		}
	}
</style>
