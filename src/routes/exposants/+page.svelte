<script lang="ts">
	import exponents from '$lib/data/exponents.json';
	import type IExponent from '$lib/data/IExponent';
	import Exponent from '../../components/exponents/Exponent.svelte';
	import Title from '../../components/exponents/Title.svelte';
	import Footer from '../../components/home/Footer.svelte';
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
	<Footer />
</main>

<style lang="scss">
	.head {
		padding: 0.01em;
		background-image: url('$lib/bg-img/exposants.png');
		background-size: 100%;
		background-repeat: no-repeat;
	}
</style>
