<template>
  <nav class="navbar" role="navigation" aria-label="dropdown navigation">
    <div class="navbar-menu">
      <div class="navbar-end container">
        <div class="navbar-item has-dropdown is-hoverable">
          <a class="navbar-link is-size-6">Home</a>

          <div class="navbar-dropdown is-right">
            <a v-for="menuitem in menuItems" :key="menuitem.name" class="navbar-item"><nuxt-link :to="menuitem.link">{{menuitem.name}}</nuxt-link></a>
            <hr class="navbar-divider" />
            <div class="navbar-item">Version 1.0</div>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
  data () {
return{
  menuItems: [
      {
        name: "Archive",
        link: "/archive"
      },
      {
        name: "Tags",
        link: "/tags"
      },
      {
        name: "About Me",
        link: "/me"
      }
    ]
}  
  }
};
</script>