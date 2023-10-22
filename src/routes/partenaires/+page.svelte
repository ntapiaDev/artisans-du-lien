<script lang="ts">
	import partners from '$lib/data/partners.json';
	import type IPartner from '$lib/data/IPartner';
	import Header from '../../components/home/Header.svelte';
	import Greta from '../../components/partners/Greta.svelte';
	import Partner from '../../components/partners/Partner.svelte';
	import Title from '../../components/partners/Title.svelte';
	import PoleEmploi from '../../components/partners/PoleEmploi.svelte';
	import Atrium from '../../components/partners/Atrium.svelte';
	import Plie from '../../components/partners/Plie.svelte';
	import Normandie from '../../components/partners/Normandie.svelte';
	import Cd76 from '../../components/partners/CD76.svelte';
	import Fse from '../../components/partners/Fse.svelte';
	import Adep from '../../components/partners/ADEP.svelte';
	import Media from '../../components/partners/Media.svelte';

	const sortPartnersByName = (array: IPartner[]) => array.sort((a, b) => a.name.localeCompare(b.name));
</script>

<main>
	<div class="head">
		<Header />
		<Title />
	</div>
	<Greta />
	<div class="grid">
		<Atrium />
		<Cd76 />
		<Normandie />
		<Fse />
		<Plie />
		<PoleEmploi />
		<Adep />
		<Media />
		<!-- {#each sortPartnersByName(partners) as partner}
			<Partner {partner} />
		{/each} -->
	</div>
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
