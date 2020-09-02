<template>
  <div>
    <b-navbar
      class="has-shadow header is-spaced"
      fixed-top="true"
      type="is-primary"
    >
      <template slot="start">
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img
            src="~assets/buefy.png"
            alt="Lightweight UI components for Vue.js based on Bulma"
          />
        </b-navbar-item>
        <b-navbar-item href="/">
          <span>Inicio</span>
        </b-navbar-item>
        <b-navbar-item href="/about"><span>Nosotros</span> </b-navbar-item>
        <b-navbar-item href="/services"><span>Servicios</span> </b-navbar-item>
        <b-navbar-item href="/blog"><span>Blog</span></b-navbar-item>
        <b-navbar-item href="/contact"><span>Contacto</span></b-navbar-item>
      </template>
    </b-navbar>

    <section>
      <nuxt />
    </section>

    <footer class="footer">
      <div class="content has-text-centered">
        <p>
          <strong>Bulma</strong> by
          <a href="https://jgthms.com">Jeremy Thomas</a>. The source code is
          licensed
          <a href="http://opensource.org/licenses/mit-license.php">MIT</a>. The
          website content is licensed
          <a href="http://creativecommons.org/licenses/by-nc-sa/4.0/"
            >CC BY NC SA 4.0</a
          >.
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>
