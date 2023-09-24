<script lang="ts">
	let absoluteValue = 0;
	let scrollY = 0;
	let section: HTMLElement;

	$: if (scrollY) absoluteValue = getAbsoluteValue();

	const getAbsoluteValue = () => {
		const width = 400; //Attraper la vraie valeur??
		const rect = section.getBoundingClientRect();
		const positionPercent = ((rect.height - rect.y) / rect.height) * 100;
		const absoluteValue = - width + (positionPercent / 100) * width;
		return absoluteValue < 0 ? (absoluteValue > - width ? absoluteValue : - width) : 0;
	};
</script>

<svelte:window bind:scrollY={scrollY} />

<section bind:this={section}>
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

		img {
			height: 100vh;
			position: absolute;

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
