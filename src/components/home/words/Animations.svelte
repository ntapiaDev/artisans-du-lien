<script lang="ts">
	export let absoluteValue: number;
</script>

<div class="warp" style="top: calc({absoluteValue * 2}px + 62vh) ; opacity: {1 - (absoluteValue / -375)}">
	<span class="warp__0">A</span>
	<span class="warp__1">n</span>
	<span class="warp__2">i</span>
	<span class="warp__3">m</span>
	<span class="warp__4">a</span>
	<span class="warp__5">t</span>
	<span class="warp__6">i</span>
	<span class="warp__7">o</span>
	<span class="warp__8">n</span>
	<span class="warp__9">s</span>
</div>

<style lang="scss">
	.warp {
		position: absolute;
        left: 18%;
		font-size: 4em;
		color: var(--primary-color);
		font-weight: bold;
		text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
		@media screen and (max-width: 768px) {
			left: 10%;
			font-size: 2em;
			transform: translateY(10vh);
			z-index: 999;
		}
	}

	[class*='warp__'] {
		position: absolute;
	}

	.warp__0 {
		transform-origin: 50% 43px;
		transform: translate(-5.5144px, 80.3241px) rotate(0.324359rad);
	}

	.warp__1 {
		transform-origin: 50% 43px;
		transform: translate(33.4452px, 89.70920000000001px) rotate(0.139619rad);
	}

	.warp__2 {
		transform-origin: 50% 43px;
		transform: translate(76.4433px, 92.0627px) rotate(0.003218rad);
	}

	.warp__3 {
		transform-origin: 50% 43px;
		transform: translate(99.9426px, 88.9793px) rotate(-0.145719rad);
	}

	.warp__4 {
		transform-origin: 50% 43px;
		transform: translate(159.8772px, 78.0687px) rotate(-0.292874rad);
	}

	.warp__5 {
		transform-origin: 50% 43px;
		transform: translate(195.147px, 67.7362px) rotate(-0.373975rad);
	}

	.warp__6 {
		transform-origin: 50% 43px;
		transform: translate(219.9035px, 57.7825px) rotate(-0.434253rad);
	}

	.warp__7 {
		transform-origin: 50% 43px;
		transform: translate(240.46159999999998px, 43.8023px) rotate(-0.504195rad);
	}

	.warp__8 {
		transform-origin: 50% 43px;
		transform: translate(272.3902px, 22.7457px) rotate(-0.593772rad);
	}

	.warp__9 {
		transform-origin: 50% 43px;
		transform: translate(307.2537px, 0.6687000000000012px) rotate(-0.680925rad);
	}
</style>
