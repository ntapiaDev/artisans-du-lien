<script lang="ts">
	export let absoluteValue: number;
</script>

<div class="warp" style="top: calc({absoluteValue * 1.5}px + 2vh); opacity: {1 - (absoluteValue / -375)}">
	<span class="warp__0">T</span>
	<span class="warp__1">a</span>
	<span class="warp__2">b</span>
	<span class="warp__3">l</span>
	<span class="warp__4">e</span>
	<span class="warp__5">s</span>
	<span class="warp__6" />
	<span class="warp__7">R</span>
	<span class="warp__8">o</span>
	<span class="warp__9">n</span>
	<span class="warp__10">d</span>
	<span class="warp__11">e</span>
	<span class="warp__12">s</span>
</div>

<style lang="scss">
	.warp {
		position: absolute;
		left: 28%;
		font-size: 4em;
		color: var(--primary-color);
		font-weight: bold;
		text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
		transform: rotate(-6deg);
		@media screen and (max-width: 768px) {
			left: 10%;
			font-size: 2em;
			z-index: 999;
		}
	}

	[class*='warp__'] {
		position: absolute;
	}

	.warp__0 {
		transform-origin: 50% 43px;
		transform: translate(-79.2795px, 310.0107px) rotate(0.170467rad);
	}

	.warp__1 {
		transform-origin: 50% 43px;
		transform: translate(-38.7545px, 315.6576px) rotate(0.11341rad);
	}

	.warp__2 {
		transform-origin: 50% 43px;
		transform: translate(-1.2195999999999998px, 318.574px) rotate(0.030404rad);
	}

	.warp__3 {
		transform-origin: 50% 43px;
		transform: translate(39.375px, 318.0987px) rotate(-0.064203rad);
	}

	.warp__4 {
		transform-origin: 50% 43px;
		transform: translate(62.72539999999999px, 314.6907px) rotate(-0.168258rad);
	}

	.warp__5 {
		transform-origin: 50% 43px;
		transform: translate(97.124px, 307.2082px) rotate(-0.271357rad);
	}

	.warp__6 {
		transform-origin: 50% 43px;
		transform: translate(127.91239999999999px, 297.7285px) rotate(-0.303265rad);
	}

	.warp__7 {
		transform-origin: 50% 43px;
		transform: translate(159.4913px, 286.9434px) rotate(-0.251104rad);
	}

	.warp__8 {
		transform-origin: 50% 43px;
		transform: translate(203.2297px, 278.5859px) rotate(-0.157539rad);
	}

	.warp__9 {
		transform-origin: 50% 43px;
		transform: translate(240.03500000000003px, 274.0291px) rotate(-0.076182rad);
	}

	.warp__10 {
		transform-origin: 50% 43px;
		transform: translate(283.2503px, 272.121px) rotate(-0.020768rad);
	}

	.warp__11 {
		transform-origin: 50% 43px;
		transform: translate(323.2543px, 272.2092px) rotate(0.027409rad);
	}

	.warp__12 {
		transform-origin: 50% 43px;
		transform: translate(358.3859px, 274.0253px) rotate(0.082818rad);
	}
</style>
