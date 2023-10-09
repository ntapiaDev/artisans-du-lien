<script lang="ts">
	export let absoluteValue: number;
</script>

<div class="warp" style="right: calc({absoluteValue * 3}px + 64%) ; opacity: {1 - (absoluteValue / -375)}">
    S'éveiller, s'engager
</div>

<style lang="scss">
    div {
        position: absolute;
        top: 76%;
		font-size: 2.5em;
		color: var(--primary-color);
		font-weight: bold;
		text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        z-index: 999;

        @media screen and (max-width: 768px) {
            width: 100%;
            top: 88%;
			font-size: 2em;
            transform: translateX(75%);
		}
    }
</style>
