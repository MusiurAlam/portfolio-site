<div class="notfound_container">
    <h1>404</h1>
    <h2>Page not found!</h2>
</div>

<style lang="scss">
    @import "../app.scss";

    .notfound_container {
        @extend .section, .container;
        h1 {
            font-size: clamp(4rem, 3vw, 9rem);
            font-weight: 900;
            color: #b30e0e;
        }

        h2 {
            font-size: clamp(1rem, 2vw, 3rem);
            font-weight: 800;
            color: #000;
        }
    }
</style>
