<div class="home_container">
    <h1>Welcome Everyone!</h1>
    <p>This is a starter project to start with Svelte and SASS/SCSS</p>
</div>

<style lang="scss">
    @import "../app.scss";

    .home_container {
        @extend .container, .section;

        text-align: center;

        h1 {
            font-size: clamp(1.3rem, 3vw, 6rem);
            color: orangered;
            font-weight: 900;
            margin-bottom: 3rem;
        }

        p {
            color: gray;
        }
    }
</style>
