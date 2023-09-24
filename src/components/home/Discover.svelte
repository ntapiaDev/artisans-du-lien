<div class="container">
    <div class="card">
        <div class="image image-1"></div>
        <h3 class="secondary-card round">Le programme</h3>
        <p>Découvrez les temps forts de la journée : les intervenants, tables rondes, projections, animations et ateliers.</p>
        <a href="" class="secondary-card round">Découvrir <img src="icons/violet-arrow.png" alt=""></a>
    </div>
    <div class="card">
        <div class="image image-2"></div>
        <h3 class="primary-card round">Les exposants</h3>
        <p>Plus d'une trentaine de partenaires ont répondu présents pour vous faire découvrir leurs services et produits.</p>
        <a href="" class="primary-card round">Découvrir <img src="icons/orange-arrow.png" alt=""></a>
    </div>
    <div class="card">
        <div class="image image-3"></div>
        <h3 class="secondary-card round">Les employeurs</h3>
        <p>Retrouvez les contacts des employeurs et structures présentes sur le salon.</p>
        <a href="" class="secondary-card round">Découvrir <img src="icons/violet-arrow.png" alt=""></a>
    </div>
</div>

<style lang="scss">
    .container {
        padding: 1em;
        display: grid;
        grid-template-columns: repeat(3, 1FR);
        gap: 1em;
        @media screen and (max-width: 1280px) {
            grid-template-columns: repeat(2, 1FR);
        }
        @media screen and (max-width: 768px) {
            grid-template-columns: repeat(1, 1FR);
        }

        .card {
            display: flex;
            flex-direction: column;
            align-items: flex-end;

            &:nth-child(odd) {
                color: var(--primary-color);
                background-color: var(--secondary-color);
            }
            &:nth-child(even) {
                color: var(--secondary-color);
                background-color: var(--primary-color);
            }

            .image {
                width: 100%;
                aspect-ratio: 2/1;
                background-size: cover;
                background-position: center;
            }
            .image-1 {
                background-image: url('../../../static/photos/program.png');
            }
            .image-2 {
                background-image: url('../../../static/photos/exponents.png');
            }  
            .image-3 {
                background-image: url('../../../static/photos/employers.png');
            }

            h3 {
                width: 100%;
                font-size: 2em;
                text-align: center;
            }
            .round {
                border-radius: 1em;
            }

            p {
                padding: 1em;
            }
            
            a {
                width: 125px;
                margin: 0.5em;
                padding: 0.5em;
                margin-top: auto;
                text-decoration: none;
                display: flex;
                justify-content: center;
                align-items: center;
                gap: 0.5em;

                img {
                    width: 25px;
                }
            }
        }
    }
</style>