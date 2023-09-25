<script lang="ts">
	export let absoluteValue: number;
</script>

<div class="warp" style="top: calc({absoluteValue * 2.2}px + 60vh); opacity: {1 - (absoluteValue / -375)}">
	<span class="warp__0">P</span>
	<span class="warp__1">r</span>
	<span class="warp__2">o</span>
	<span class="warp__3">j</span>
	<span class="warp__4">e</span>
	<span class="warp__5">c</span>
	<span class="warp__6">t</span>
	<span class="warp__7">i</span>
	<span class="warp__8">o</span>
	<span class="warp__9">n</span>
	<span class="warp__10">s</span>
</div>

<style lang="scss">
	.warp {
		position: absolute;
		left: 43%;
		font-size: 4em;
		color: var(--primary-color);
		font-weight: bold;
		text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
		@media screen and (max-width: 768px) {
			left: 10%;
			font-size: 2em;
			transform: translateY(-58vh);
			z-index: 999;
		}
	}

	[class*='warp__'] {
		position: absolute;
	}

	.warp__0 {
		transform-origin: 50% 43px;
		transform: translate(-2.9339000000000013px, 52.449px) rotate(0.032595rad);
	}

	.warp__1 {
		transform-origin: 50% 43px;
		transform: translate(38.8677px, 55.0607px) rotate(0.108215rad);
	}

	.warp__2 {
		transform-origin: 50% 43px;
		transform: translate(71.748px, 60.2881px) rotate(0.186011rad);
	}

	.warp__3 {
		transform-origin: 50% 43px;
		transform: translate(108.3971px, 66.6787px) rotate(0.253424rad);
	}

	.warp__4 {
		transform-origin: 50% 43px;
		transform: translate(128.6986px, 74.7426px) rotate(0.321333rad);
	}

	.warp__5 {
		transform-origin: 50% 43px;
		transform: translate(162.2346px, 87.1346px) rotate(0.40683rad);
	}

	.warp__6 {
		transform-origin: 50% 43px;
		transform: translate(193.1476px, 100.1961px) rotate(0.482558rad);
	}

	.warp__7 {
		transform-origin: 50% 43px;
		transform: translate(216.5693px, 112.57390000000001px) rotate(0.545423rad);
	}

	.warp__8 {
		transform-origin: 50% 43px;
		transform: translate(234.9066px, 129.2853px) rotate(0.620509rad);
	}

	.warp__9 {
		transform-origin: 50% 43px;
		transform: translate(263.5605px, 153.9003px) rotate(0.716275rad);
	}

	.warp__10 {
		transform-origin: 50% 43px;
		transform: translate(296.0398px, 180.0428px) rotate(0.80398rad);
	}
</style>
