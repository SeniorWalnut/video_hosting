<template>
  <main class="main-wrapper">
    <b-navbar type="is-primary">
      <template slot="brand">
        <b-navbar-item tag="nuxt-link" :to="{ path: '/' }">
          <img
            src=""
            alt="video_host"
          >
        </b-navbar-item>
      </template>
      <template slot="end">
        <b-navbar-item tag="div">
          <div class="buttons">
            <a class="button is-primary">
                <strong>Sign up</strong>
            </a>
            <a class="button is-light">
                Log in
            </a>
            <button class="button is-light">
              <b-icon
                pack="mdi"
                icon="settings"
                type="is-medium"
              >
              </b-icon>
              <!-- <span>Finish</span> -->
            </button>
        </div>
        </b-navbar-item>
      </template>
    </b-navbar>

    <nuxt />
  </main>
</template>
<script>

export default {
}
</script>
