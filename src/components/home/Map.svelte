<script>
    import { onMount } from 'svelte';

    onMount(() => {
        const map = L.map('map').setView([49.428735, 1.080065], 17);
        L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png').addTo(map);

        const icon = L.icon({
            iconUrl: 'icons/marker.png',
            iconAnchor: [12, 40]
        });

        const marker = L.marker([49.428735, 1.080065], { icon: icon }).addTo(map);
    });
</script>

<svelte:head>
    <link rel="stylesheet"
        href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
        integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
        crossorigin=""/>
    <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
        integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
        crossorigin="">
    </script>
</svelte:head>

<div id="map">
    <div class="primary-card">Venir à l'Atrium</div>
</div>

<style lang="scss">
    #map {
        width: 350px;
        height: 350px;
        position: relative;

        div {
            position: absolute;
            top: 0;
            right: 0;
            padding: 0.25em 1em;
            font-size: 1.5em;
            z-index: 999;
        }
    }
</style>