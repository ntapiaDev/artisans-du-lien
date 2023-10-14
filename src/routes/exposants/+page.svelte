<script lang="ts">
	import exponents from '$lib/data/exponents.json';
	import type IExponent from '$lib/data/IExponent';
	import Exponent from '../../components/exponents/Exponent.svelte';
	import Title from '../../components/exponents/Title.svelte';
	import Header from '../../components/home/Header.svelte';

	const sortExponentsByName = (array: IExponent[]) => array.sort((a, b) => a.name.localeCompare(b.name));
</script>

<main>
	<div class="head">
		<Header />
		<Title />
	</div>
	<div class="grid">
		{#each sortExponentsByName(exponents) as exponent}
			<Exponent {exponent} />
		{/each}
	</div>
</main>

<style lang="scss">
	.head {
		padding: 0.01em;
		background-image: url('$lib/bg-img/exposants.png');
		background-position: center;
		background-size: cover;
		background-repeat: no-repeat;
	}

	.grid {
		margin: 1em;
		display: grid;
		grid-template-columns: repeat(2, 1FR);
		gap: 1em;

		@media screen and (max-width: 768px) {
			display: block;
		}
	}
</style>
