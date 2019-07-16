<template>
  <div>
    <nav
      class="navbar header has-shadow is-primary"
      role="navigation"
      aria-label="main navigation"
    >
      <div class="navbar-brand">
        <a class="navbar-item" href="/">
          Design Influences
        </a>

        <div class="navbar-burger">
          <span aria-hidden="true" />
          <span aria-hidden="true" />
          <span aria-hidden="true" />
        </div>
      </div>

      <div id="main-menu" class="navbar-menu">
        <div class="navbar-start">
          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link">Imagine</a>
            <div class="navbar-dropdown">
              <a class="navbar-item">Resources</a>
              <a class="navbar-item">Theory</a>
              <a class="navbar-item">Research</a>
              <a class="navbar-item">Strategy</a>
            </div>
          </div>
          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link">Design</a>
            <div class="navbar-dropdown">
              <a class="navbar-item">Identity</a>
              <a class="navbar-item">Print</a>
              <a class="navbar-item">Web</a>
              <a class="navbar-item">Type</a>
            </div>
          </div>
          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link">Build</a>
            <div class="navbar-dropdown">
              <a class="navbar-item">People</a>
              <a class="navbar-item">Relationships</a>
              <a class="navbar-item">Community</a>
            </div>
          </div>
        </div>

        <div class="navbar-end">
          <a class="navbar-item">About</a>
          <a class="navbar-item">Journal</a>
          <a class="navbar-item">Work</a>
          <a class="navbar-item">Resources</a>
        </div>
      </div>
    </nav>

    <section class="main-content columns">
      <aside class="column is-2 section">
        <p class="menu-label is-hidden-touch">
          General
        </p>
        <ul class="menu-list">
          <li v-for="(item, key) of items" :key="key">
            <nuxt-link :to="item.to" exact-active-class="is-active">
              <b-icon :icon="item.icon" /> {{ item.title }}
            </nuxt-link>
          </li>
        </ul>
      </aside>

      <div class="container column is-10">
        <nuxt />
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' }
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' }
        }
      ]
    }
  }
}
</script>
