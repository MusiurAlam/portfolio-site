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
