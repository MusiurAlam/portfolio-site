<script>
  export let properties = {
    title: "Privacy Pie",
  };

  const { title } = properties;
</script>

<div class="works_cards">
  <img src="/icons/ActiveTick__ICON.svg" alt="active_check" class="" />
  <p>{title}</p>
  <img src="/icons/GrayRightArray.svg" alt="right_arrow" class="" />
</div>

<style lang="scss">
  @import "./works_cards.scss";
</style>
