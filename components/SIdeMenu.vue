<template>
  <div class="side-menu">
    <div class="side-menu__wrapper">
      <menu-links
        :links="sideMenuLinks"
      />
    </div>
  </div>
</template>
<script>
import MenuLinks from './MenuLinks'

export default {
  components: { MenuLinks },
  computed: {
    sideMenuLinks () {
      return [
        { name: "Prodfile", icon: "settings", children: [] },
        { name: "Videos", icon: "settings", children: [
          { name: "Liked", icon: "settings", children: [] },
          { name: "Commented", icon: "settings", children: [] },
          { name: "Favourite", icon: "settings", children: [] },
          { name: "Disliked", icon: "settings", children: [] }
        ] },
        { name: "My Subs", icon: "settings", children: [] },
        { name: "My videos", icon: "settings", children: [] }
      ]
    }
  }
}
</script>
