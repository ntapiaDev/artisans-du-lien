<script lang="ts">
	import type IExponent from '$lib/data/IExponent';

	export let exponent: IExponent;
</script>

<div class="card">
	<div class="title">
		<h3>
			{exponent.name}
		</h3>
		<span>
			{#if exponent.title}
				"{exponent.title}"
			{/if}
		</span>
	</div>
	<div class="content">
		<img src={'exponents/' + exponent.icon} alt={exponent.name} />
		<div>{exponent.description}</div>
	</div>
	<div class="contact">
		<span>
			{#if exponent.contact && typeof exponent.contact === 'string'}
				<a href="mailto:{exponent.contact}">
					<span class="email">
						<img src="icons/email.png" alt="email" class="e" />{exponent.contact}
					</span>
				</a>
			{:else if exponent.contact && Array.isArray(exponent.contact)}
				<span class="double">
					{#each exponent.contact as contact}
						<a href="mailto:{contact}">
							<span class="email">
								<img src="icons/email.png" alt="email" class="e" />{contact}
							</span>
						</a>
					{/each}
				</span>
			{/if}
		</span>
		<span>
			{#if exponent.website}
				<a href={exponent.website} target="_blank">
					<span class="website">
						<img src="icons/website.png" alt="site internet" class="w" />Site internet
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
			background-color: var(--secondary-color);
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
				color: var(--primary-color);
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

				.double {
					margin-right: 1em;

					@media screen and (max-width: 768px) {
						display: flex;
						flex-direction: column;
					}
				}

				a {
					color: #ffffff;
					display: block;
					width: 100%;
				}

				.email,
				.website {
					padding: 0.5em 1em;
					background-color: var(--secondary-color);
					border-radius: 2em;
					display: flex;
					align-items: center;
					justify-content: center;
					gap: 1em;

					img.e {
						width: 45px;
						height: 30px;
					}

					img.w {
						width: 30px;
						height: 30px;
					}
				}
			}
		}
	}
</style>
