<script>
  //to get global classes
  // from anywhere directly in HTML
  import "../app.scss";
  import Footer from "../components/footer/footer.svelte";
  import Nav from "../components/navbar/nav.svelte";
</script>

<Nav />

<slot />

<Footer />
