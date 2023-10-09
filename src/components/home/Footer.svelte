<script>
	import Map from "./Map.svelte";
</script>
<footer>
    <div>
        <div>
            <h3>Greta Rouen Maritime</h3>
            <div>Antenne de Grand Quevilly</div>
            <div>17 avenue Franklin Roosevelt</div>
            <div>76120 Grand Quevilly</div>
            <div>02.32.11.01.06</div>
            <div><a href="mailto:grand-quevilly@greta-rouen.fr?subject=Artisans du lien">grand-quevilly@greta-rouen.fr</a></div>
        </div>
        <div class="footer">Les artisans du lien - Lundi 13 novembre 2023 à L'ATRIUM</div>
    </div>
    <Map />
</footer>

<style lang="scss">
    footer {
        color: var(--secondary-color);
        background-color: var(--background-color);
        display: flex;
        @media screen and (max-width: 1024px) {
            flex-direction: column-reverse;
            align-items: center;
        }

        & > div {
            flex-grow: 1;
            display: flex;
            flex-wrap: wrap;
            gap: 5em;

            & > div {
                padding: 1em;

                h3 {
                    font-size: 2em;
                }
            }
        }

        .footer {
            width: 100%;
            height: 50px;
            margin-top: auto;
            color: #ffffff;
            background-color: var(--secondary-color);
            display: flex;
            justify-content: center;
            align-items: center;
        }
    }
</style>