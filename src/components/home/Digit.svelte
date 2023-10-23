<script lang="ts">
	export let digit: number;
    export let update: number;

	let current = digit;
    let old = digit;
	
	let hasTransition = true;
	let x = -40;

    $: if (update) {
        if (digit === old) {
            hasTransition = false;
            x = -40;
            current = digit;
		} else {
            hasTransition = true;
            x = 0;
            old = digit;
		}
    }
</script>

<div class={hasTransition ? 'with-transition' : ''} style="top: {x}px;">
	<div>{digit}</div>
	<div>{current}</div>
</div>

<style lang="scss">
	div {
		position: relative;
		width: 20px;
		height: 80px;
		font-weight: bold;
		font-size: 1.25em;
		background-color: var(--primary-color);
		color: var(--secondary-color);

		display: flex;
		flex-direction: column;
		align-items: center;

		&.with-transition {
			transition: 0.5s;
		}
	}
</style>
