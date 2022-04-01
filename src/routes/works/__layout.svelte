<script>
  import Submenu from "../../components/works/submenu.svelte";
</script>

<div class="container">
  <div class="settings_container">
    <Submenu />

    <slot />
  </div>
</div>

<style lang="scss">
  @import "../../app.scss";

  .settings_container {
    display: flex;

    @extend .section;
  }
</style>
