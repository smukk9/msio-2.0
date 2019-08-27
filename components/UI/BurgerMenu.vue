<template>
  <nav class="is-overlay">
    <div class="navbar-menu container ">
            <div class="navbar-end">
        <b-dropdown v-model="navigation" position="is-bottom-left" aria-role="menu">
          <a  class="navbar-item has-background-white" slot="trigger" role="button">
            <span >Menu</span>
            <b-icon icon="menu-down"></b-icon>
          </a>
          <b-dropdown-item has-link v-for="menuItem in menuItems" is-size-2 :key="menuItem" aria-role="menuitem">
            <a :href=menuItem.link target="_self">
                            <b-icon icon=menuItem.icon></b-icon>
                            {{menuItem.name}}
                        </a>
          </b-dropdown-item>
          <hr class="dropdown-divider" aria-role="menuitem" />
          <b-dropdown-item value="settings">
            <b-switch :value="true" type="is-success">Dark Mode</b-switch>
          </b-dropdown-item>
        </b-dropdown>
            </div>
    </div>
</nav>

</template>

<script>
export default {
  data() {
    return {
      "navigation": "home",
      menuItems: [
      {
          "name": "Home",
          "key": "home",
          "icon": "home",
          "link": "/"

        },
        {
          "name": "Archive",
          "key": "archive",
          "icon": "book-open",
          "link": "/archive"

        },
        {
          "name": "Tags",
          "key": "tag",
          "icon": "tags",
          "link": "/tags"
        },
        {
          "name": "About Me",
          "key": "about",
          "icon": "user",
          "link": "/me"
        },
        {
          "name": "Logout",
          "key": "logout",
          "icon": "logout",
          "link": "/logout"
        }
      ]
    };
  }
};
</script>