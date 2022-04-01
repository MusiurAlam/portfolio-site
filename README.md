# Hi, there!
## This is Musiur Alam Opu

This is a starter project I have created using Svelte and SCSS.<br><br>

In order to install the project in your local machine run the commands below: <br>

  ```
    1. git clone https://github.com/MusiurAlam/test-kit.git
    2. cd test-kit
    3. yarn install / npm install
    4. yarn start / npm start
  ```
<br>

Visit the deplyoed site: `https://test-kit-rouge.vercel.app/`
<br>
<br>

## You will find in this project
- Basic routes such as home, about, settings etc. <br>
  index.svelte
  ```
  
    <div class="home_container">
        <h1>Welcome Everyone!</h1>
        <p>This is a start project to start with Svelte and SASS/SCSS</p>
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


  ```
- Nested routes like settings > profile, settings > notifications.
- Layouts for root/nested routes.
- Custom Not Found (404) page. <br>
  __error.svelte
  ```
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

  ```
- Integrated Scss both by importing external and within components.
- app.scss for global styling which is imported in <br> __layout.svelte
  
  
  ```
    <script>
    //to get global classes
    // from anywhere directly in HTML
    import "../app.scss";
    </script>

    <div class="layout">
        <nav class="nav container">
            <h1><a href="/">Musiur</a></h1>
            <div>
                <a href="/">Home</a>
                <a href="/about">About</a>
                <a href="/settings">Settings</a>
            </div>
        </nav>
    </div>

    <slot />

    <footer>
    <p>
        Created by <span
        ><a href="https://github.com/MusiurAlam" target="_blank" rel="noopener"
            >@musiur_alam_opu</a
        ></span
        >
    </p>
    </footer>

    <style lang="scss">
    @import "../app.scss";

    nav {
        background-color: black;

        display: flex;
        justify-content: space-between;
        align-items: center;

        div {
            padding: 2rem 0rem;
            display: flex;
            flex-direction: row;
            justify-content: flex-end;
            column-gap: 1rem;
        }

        a {
            color: #fff;
            text-decoration: none;
        }

        h1 {
            a {
                font-weight: 600;
                background: -webkit-linear-gradient(60deg, #ff0202, #ffce72);
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
            }
        }
    }

    footer {
        @extend .container, .section;

        position: absolute;
        left: 0;
        right: 0;
        bottom: 0;
        text-align: center;

        p {
        font-weight: 600;

            span,
            a {
                color: orangered;
                text-decoration: none;

                &:hover {
                color: #007bff;
                }
            }
        }
    }
    </style>



  ```

If you have faced any problem then contact with me `musiuralamo@gmail.com`
<br> 
<br>
Thank you very much.