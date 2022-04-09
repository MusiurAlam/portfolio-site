<script>
  export let properties = {
    label: "Develop",
    icon: "git_icon",
    circularIcon: "",
    type: "label",
  };

  const { label, icon, circularIcon, type } = properties;
</script>

<div class="git_label_main_container">
  <div>
    {#if circularIcon}
      <img src={circularIcon} alt="right_arrow" />
    {/if}
  </div>

  <p
    class={type === "label" ? "git_label__container" : "git_command__container"}
  >
    {#if icon}
      <img src={icon} alt="git" />
    {/if}

    {#if label}
      <span>{label}</span>
    {/if}
  </p>
</div>

<style lang="scss">
  @import "./git_label.scss";
</style>
