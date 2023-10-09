<script lang="ts">
	import partners from '$lib/data/partners.json';
	import type IPartner from '$lib/data/IPartner';

	import Title from '../../components/partners/Title.svelte';
	import Footer from '../../components/home/Footer.svelte';
	import Header from '../../components/home/Header.svelte';

	const sortPartnersByName = (array: IPartner[]) => array.sort((a, b) => a.name.localeCompare(b.name));
</script>

<main>
	<div class="head">
		<Header />
		<Title />
	</div>
	<div class="grid">
		{#each sortPartnersByName(partners) as exponent}
			<!-- <Exponent {exponent} /> -->
		{/each}
	</div>
	<Footer />
</main>

<style lang="scss">
	.head {
		padding: 0.01em;
		background-image: url('$lib/bg-img/partenaires.png');
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
