<template>
  <div class="menu-links">
    <b-menu>
      <b-menu-list>
        <b-menu-item
          v-for="(link, ind) in links"
          :key="link.name + ind"
          :icon="link.icon"
          :label="link.name"
          tag="nuxt-link"
          to="/"
        >{{ link.name }}</b-menu-item>
      </b-menu-list>
    </b-menu>
  </div>
</template>
<script>
export default {
  props: {
    links: {
      type: Array,
      default: () => []
    }
  }
}
</script>
<style>
.menu-links > * {
  font-size: 1.5rem;
}
</style>
