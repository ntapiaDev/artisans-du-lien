<script>
	import Atrium from '../components/home/Atrium.svelte';
	import Date from '../components/home/Date.svelte';
	import Discover from '../components/home/Discover.svelte';
	import Footer from '../components/home/Footer.svelte';
	import Header from '../components/home/Header.svelte';
	import Landing from '../components/home/Landing.svelte';
	import Map from '../components/home/Map.svelte';
	import Poster from '../components/home/Poster.svelte';
	import Video from '../components/home/Video.svelte';
</script>

<Video />

<main>
	<section id="landing">
		<Header />
		<Landing />
	</section>
	<section>
		<Date />
		<Atrium />
		<Poster />
		<Discover />
		<Map />
		<Footer />
	</section>
</main>

<style lang="scss">
	#landing {
		min-height: 100vh;
	}
</style>
