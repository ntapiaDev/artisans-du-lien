<script>
	import Atrium from '../components/home/Atrium.svelte';
	import Date from '../components/home/Date.svelte';
	import Discover from '../components/home/Discover.svelte';
	import Footer from '../components/home/Footer.svelte';
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
		<div class="logos">
			<img src="logos/normandie.png" alt="" />
			<img src="logos/fse.png" alt="" />
			<img src="logos/76.png" alt="" />
		</div>
	</section>
	<section>
		<Date />
		<Atrium />
		<Poster />
		<Discover />
		<Footer />
	</section>
</main>

<style lang="scss">
	#landing {
		min-height: 100svh;
		position: relative;

		.logos {
			bottom: 2em;
			right: 1em;
			position: absolute;
			display: flex;
			flex-direction: column;
			gap: 1em;

			@media screen and (max-width: 768px) {
				flex-direction: row;
			}

			img {
				height: 100px;
				
				@media screen and (max-width: 768px) {
					height: 50px;
				}
			}
		}
	}
</style>
