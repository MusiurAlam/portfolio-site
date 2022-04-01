<div class="container">
    <div class="settings_container">
        <div class="submenu">
            <h2>Submenu</h2>
            <a href="/settings">Settings</a>
            <a href="/settings/profile">Profile</a>
            <a href="/settings/notifications">Notifications</a>
        </div>

        <slot />
    </div>
</div>

<style lang="scss">
    @import "../../styles/settingsNav.scss";

    h2 {
        border-bottom: 1px solid lightgray;
    }
</style>
