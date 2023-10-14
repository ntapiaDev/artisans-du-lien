<script lang="ts">
	import type IPartner from '$lib/data/IPartner';

	export let partner: IPartner;
</script>

<div class="card">
	<div class="title">
		<h3>
			{partner.name}
		</h3>
		<span>
			{#if partner.title}
				"{partner.title}"
			{/if}
		</span>
	</div>
	<div class="content">
		<img src={'partners/' + partner.icon} alt={partner.name} />
		<div>{partner.description}</div>
	</div>
	<div class="contact">
		<span></span>
		<span>
			{#if partner.website}
				<a href={partner.website} target="_blank">
					<span class="website">
						<img src="icons/website_p.png" alt="site internet" />Site internet
					</span>
				</a>
			{/if}
		</span>
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
				white-space: nowrap;

				@media screen and (max-width: 768px) {
					font-size: 1.5em;
				}
			}

			span {
				font-size: 1.5em;
				color: #ffffff;
				text-align: end;

				@media screen and (max-width: 768px) {
					font-size: 1em;
					text-align: center;
				}
			}
		}

		.content {
			padding: 1em;
			text-align: justify;

			img {
				float: left;
				margin: 0 1em 0 0;
				max-width: 200px;
				max-height: 100px;
			}
		}

		.contact {
			margin-top: auto;
			padding: 0 1em 1em 1em;
			display: flex;
			justify-content: space-between;

			@media screen and (max-width: 768px) {
				flex-direction: column;
				gap: 1em;
			}

			span {
				display: flex;
				gap: 1em;

				@media screen and (max-width: 768px) {
					width: 100%;
				}

				a {
					color: #ffffff;
					display: block;
					width: 100%;
				}

				.website {
					padding: 0.5em 1em;
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
	}
</style>
