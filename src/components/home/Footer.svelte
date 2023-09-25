<script>
	import Map from "./Map.svelte";
</script>
<footer>
    <div>
        <div>
            <h3>A propos de nous</h3>
            <div>Contenu à ajouter</div>
            <div>Contenu à ajouter</div>
        </div>
        <div>
            <h3>A propos de nous</h3>
            <div>Contenu à ajouter</div>
            <div>Contenu à ajouter</div>
        </div>
        <div class="footer">Blabla</div>
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