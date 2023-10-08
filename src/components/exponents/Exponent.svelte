<script lang="ts">
	import type IExponent from '$lib/data/IExponent';

	export let exponent: IExponent;
</script>

<div>
	<img src={'exponents/' + exponent.icon} alt="" />
	<div>
		{exponent.name}
	</div>
	<div>
		{exponent.title}
	</div>
	<div>
		{exponent.description}
	</div>
	<div>
		{#if typeof exponent.contact === 'string'}
			<a href="mailto:{exponent.contact}">{exponent.contact}</a>
		{:else if Array.isArray(exponent.contact)}
			{#each exponent.contact as contact}
				<a href="mailto:{contact}">{contact}</a>
			{/each}
		{/if}
	</div>
	<div>
		{#if exponent.website}
			<a href={exponent.website} target="_blank">Site internet</a>
		{/if}
	</div>
</div>

<style lang="scss">
	img {
		height: 100px;
	}

	a {
		display: block;
	}
</style>
