<script lang="ts">
	import Animations from "./words/Animations.svelte";
	import Atelier from "./words/Atelier.svelte";
	import Projections from "./words/Projections.svelte";
	import Rencontres from "./words/Rencontres.svelte";
	import TablesRondes from "./words/TablesRondes.svelte";

	let absoluteValue = 0;
	let scrollY = 0;
	let section: HTMLElement;

	$: if (scrollY) absoluteValue = getAbsoluteValue();

	const getAbsoluteValue = () => {
		const width = 375; //Attraper la vraie valeur??
		const rect = section.getBoundingClientRect();
		const positionPercent = ((rect.height - rect.y + 16) / rect.height) * 100;
		let absoluteValue = -width + (positionPercent / 100) * width;
		// if (absoluteValue > 0) absoluteValue = -absoluteValue;
		return absoluteValue < 0 ? (absoluteValue > -width ? absoluteValue : -width) : 0;
	};
</script>

<svelte:window bind:scrollY />

<section bind:this={section}>
	<div>
		<div class="primary-card">Les artisans du lien</div>
		<div class="secondary-card">Chez vous au quotidien</div>
	</div>
	<Animations {absoluteValue} />
	<Atelier {absoluteValue} />
	<Projections {absoluteValue} />
	<Rencontres {absoluteValue} />
	<TablesRondes {absoluteValue} />
	<img src="icons/man.png" alt="" style="left: {absoluteValue}px" class="man" />
	<img src="icons/woman.png" alt="" style="right: {absoluteValue}px" class="woman" />
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
			z-index: 9;
			div {
				padding: 0 0.5em;
				font-size: 3em;
				@media screen and (max-width: 768px) {
					font-size: 1.5em;
				}
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
			@media screen and (max-width: 768px) {
				&.man {
					transform: translate(-125px);
				}
				&.woman {
					transform: translate(125px);
				}
			}

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
