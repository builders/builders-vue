<template>
  <nav
    class="navbar header has-shadow is-primary"
    role="navigation"
    aria-label="main navigation"
  >
    <div class="container">
      <div class="navbar-brand">
        <a class="navbar-item" href="/">
          Design Influences
        </a>

        <div
          class="navbar-burger"
          :class="{ 'is-active': showNav }"
          @click="showNav = !showNav"
        >
          <span aria-hidden="true" />
          <span aria-hidden="true" />
          <span aria-hidden="true" />
        </div>
      </div>

      <div id="main-menu" class="navbar-menu" :class="{ 'is-active': showNav }">
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
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      showNav: false
    }
  }
}
</script>
