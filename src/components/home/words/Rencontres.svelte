<script lang="ts">
	export let absoluteValue: number;
    
</script>

<div class="warp" style="top: calc({absoluteValue * 1.8}px + 55vh); opacity: {1 - (absoluteValue / -375)}">
	<span class="warp__0">R</span>
	<span class="warp__1">e</span>
	<span class="warp__2">n</span>
	<span class="warp__3">c</span>
	<span class="warp__4">o</span>
	<span class="warp__5">n</span>
	<span class="warp__6">t</span>
	<span class="warp__7">r</span>
	<span class="warp__8">e</span>
	<span class="warp__9">s</span>
</div>

<style lang="scss">
	.warp {
		position: absolute;
		left: 62%;
		font-size: 4em;
		color: var(--primary-color);
		font-weight: bold;
		text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
		@media screen and (max-width: 768px) {
			left: -10%;
			font-size: 2em;
			transform: translateY(2vh) rotate(-15deg);
			z-index: 999;
		}
	}

	[class*='warp__'] {
		position: absolute;
	}

	.warp__0 {
		transform-origin: 50% 43px;
		transform: translate(39.1197px, 69.1833px) rotate(-0.874433rad);
	}

	.warp__1 {
		transform-origin: 50% 43px;
		transform: translate(73.9916px, 43.6165px) rotate(-0.505328rad);
	}

	.warp__2 {
		transform-origin: 50% 43px;
		transform: translate(107.798px, 32.1002px) rotate(-0.101806rad);
	}

	.warp__3 {
		transform-origin: 50% 43px;
		transform: translate(150.1543px, 34.1802px) rotate(0.191556rad);
	}

	.warp__4 {
		transform-origin: 50% 43px;
		transform: translate(182.0737px, 44.2043px) rotate(0.370986rad);
	}

	.warp__5 {
		transform-origin: 50% 43px;
		transform: translate(215.304px, 61.1301px) rotate(0.505089rad);
	}

	.warp__6 {
		transform-origin: 50% 43px;
		transform: translate(252.841px, 79.2013px) rotate(0.589194rad);
	}

	.warp__7 {
		transform-origin: 50% 43px;
		transform: translate(273.8408px, 96.28139999999999px) rotate(0.646106rad);
	}

	.warp__8 {
		transform-origin: 50% 43px;
		transform: translate(298.869px, 117.4965px) rotate(0.701713rad);
	}

	.warp__9 {
		transform-origin: 50% 43px;
		transform: translate(325.4799px, 139.8308px) rotate(0.75182rad);
	}
</style>
