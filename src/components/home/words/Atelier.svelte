<script lang="ts">
	export let absoluteValue: number;
</script>

<div class="warp" style="top: calc({absoluteValue}px + 20vh); opacity: {1 - (absoluteValue / -375)}">
	<span class="warp__0">A</span>
	<span class="warp__1">t</span>
	<span class="warp__2">e</span>
	<span class="warp__3">l</span>
	<span class="warp__4">i</span>
	<span class="warp__5">e</span>
	<span class="warp__6">r</span>
	<span class="warp__7">s</span>
</div>

<style lang="scss">
	.warp {
		position: absolute;
		left: 56%;
		font-size: 4em;
		color: var(--primary-color);
		font-weight: bold;
		text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
		@media screen and (max-width: 768px) {
			left: -10%;
			font-size: 2em;
			transform: translateY(-5vh);
			z-index: 999;
		}
	}

	[class*='warp__'] {
		position: absolute;
	}

	.warp__0 {
		transform-origin: 50% 43px;
		transform: translate(68.6735px, 62.4011px) rotate(1.069627rad);
	}

	.warp__1 {
		transform-origin: 50% 43px;
		transform: translate(97.0445px, 88.24119999999999px) rotate(0.697045rad);
	}

	.warp__2 {
		transform-origin: 50% 43px;
		transform: translate(118.9434px, 104.5549px) rotate(0.424436rad);
	}

	.warp__3 {
		transform-origin: 50% 43px;
		transform: translate(152.8236px, 113.99430000000001px) rotate(0.238396rad);
	}

	.warp__4 {
		transform-origin: 50% 43px;
		transform: translate(175.4661px, 118.1353px) rotate(0.127319rad);
	}

	.warp__5 {
		transform-origin: 50% 43px;
		transform: translate(199.1384px, 120.13550000000001px) rotate(0.011261rad);
	}

	.warp__6 {
		transform-origin: 50% 43px;
		transform: translate(234.9176px, 118.53890000000001px) rotate(-0.10211rad);
	}

	.warp__7 {
		transform-origin: 50% 43px;
		transform: translate(267.0298px, 113.57939999999999px) rotate(-0.205016rad);
	}
</style>
