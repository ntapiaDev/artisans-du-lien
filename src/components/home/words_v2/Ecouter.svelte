<script lang="ts">
	export let absoluteValue: number;
</script>

<div class="warp" style="left: calc({absoluteValue * 3}px + 52%) ; opacity: {1 - (absoluteValue / -375)}">
    Écouter, s'informer
</div>

<style lang="scss">
    div {
        position: absolute;
        top: 28%;
		font-size: 2.5em;
		color: var(--primary-color);
		font-weight: bold;
		text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        z-index: 999;

        @media screen and (max-width: 768px) {
            width: 100%;
			font-size: 2em;
            transform: translateX(-20%);
		}
    }
</style>
