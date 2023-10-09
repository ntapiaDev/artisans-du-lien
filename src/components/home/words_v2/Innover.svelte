<script lang="ts">
	export let absoluteValue: number;
</script>

<div class="warp" style="right: calc({absoluteValue * 2}px + 62%) ; opacity: {1 - (absoluteValue / -375)}">
    Innover
</div>

<style lang="scss">
    div {
        position: absolute;
        top: 40%;
		font-size: 4em;
		color: var(--primary-color);
		font-weight: bold;
		text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        z-index: 999;

        @media screen and (max-width: 768px) {
			font-size: 3em;
			transform: translateX(10%);
		}
    }
</style>
