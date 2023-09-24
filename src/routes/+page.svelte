<script>
	import Atrium from '../components/home/Atrium.svelte';
import Date from '../components/home/Date.svelte';
	import Header from '../components/home/Header.svelte';
	import Landing from '../components/home/Landing.svelte';
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
	</section>
</main>

<style lang="scss">
	#landing {
		min-height: 100vh;
	}
</style>
