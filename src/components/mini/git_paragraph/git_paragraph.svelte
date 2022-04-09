<script>
  export let properties = { icon: "", text: "" };
  const { icon, text } = properties;
</script>

<div class="git_paragraph_container">
  <div>
    <img src={icon} alt="" />
  </div>
  <p>{text}</p>
</div>

<style lang="scss">
  @import "./git_paragraph.scss";
</style>
