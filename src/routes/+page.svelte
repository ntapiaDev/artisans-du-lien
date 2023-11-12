<script>
	import Atrium from '../components/home/Atrium.svelte';
	import Countdown from '../components/home/Countdown.svelte';
	import Date from '../components/home/Date.svelte';
	import Discover from '../components/home/Discover.svelte';
	import Header from '../components/home/Header.svelte';
	import Landing from '../components/home/Landing.svelte';
	import Poster from '../components/home/Poster.svelte';
	import Video from '../components/home/Video.svelte';
</script>

<Video />

<main>
	<section id="landing">
		<Header />
		<Landing />
		<aside>
			<!-- <div class="countdown_d">
				<Countdown />
			</div> -->
			<div class="logos">
				<img src="logos/normandie.png" alt="" />
				<img src="logos/fse.png" alt="" />
				<img src="logos/76.png" alt="" />
			</div>
		</aside>
	</section>
	<!-- <div class="countdown_m">
		<Countdown />
	</div> -->
	<section>
		<Date />
		<Atrium />
		<Poster />
		<Discover />
	</section>
</main>

<style lang="scss">
	#landing {
		min-height: 100svh;
		position: relative;

		aside {
			bottom: 2em;
			right: 1em;
			position: absolute;
			display: flex;
			align-items: end;
			gap: 1em;

			.countdown_d {
				@media screen and (max-width: 768px) {
					display: none;
				}
			}

			.logos {
				display: flex;
				flex-direction: column;
				gap: 1em;

				@media screen and (max-width: 768px) {
					flex-direction: row;
				}

				img {
					width: 120px;

					@media screen and (max-width: 768px) {
						width: auto;
						height: 50px;
					}
				}
			}
		}
	}

	.countdown_m {
		display: none;
		@media screen and (max-width: 768px) {
			padding: 0 1em;
			display: block;
		}
	}
</style>
