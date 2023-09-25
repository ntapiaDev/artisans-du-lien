<script lang="ts">
	let absoluteValue = 0;
	let scrollY = 0;
	let section: HTMLElement;

	$: if (scrollY) absoluteValue = getAbsoluteValue();

	const getAbsoluteValue = () => {
		const width = 375; //Attraper la vraie valeur??
		const rect = section.getBoundingClientRect();
		const positionPercent = ((rect.height - rect.y) / rect.height) * 100;
		let absoluteValue = -width + (positionPercent / 100) * width;
		if (absoluteValue > 0) absoluteValue = -absoluteValue;
		return absoluteValue < 0 ? (absoluteValue > -width ? absoluteValue : -width) : 0;
	};
</script>

<svelte:window bind:scrollY />

<section bind:this={section}>
	<div>
		<div class="primary-card">Les artisans du lien</div>
		<div class="secondary-card">Chez vous au quotidien</div>
	</div>
	<img src="icons/man.png" alt="" style="left: {absoluteValue}px" />
	<img src="icons/woman.png" alt="" style="right: {absoluteValue}px" />
	<img src="icons/waves-background.png" alt="" class="waves-bg" />
	<img src="icons/waves.png" alt="" class="waves" />
</section>

<style lang="scss">
	section {
		min-height: 100vh;
		margin-top: 1em;
		position: relative;
		overflow: hidden;

		div {
			display: flex;
			flex-direction: column;
			align-items: center;
			div {
				padding: 0 0.5em;
				font-size: 3em;
				&:nth-child(1) {
					margin-right: 2em;
				}
				&:nth-child(2) {
					margin-left: 2em;
				}
			}
		}

		img {
			height: 100vh;
			position: absolute;
			top: 0;

			&.waves,
			&.waves-bg {
				width: 100%;
				z-index: -1;
			}
			&.waves {
				top: 110px;
			}
		}
	}
</style>
