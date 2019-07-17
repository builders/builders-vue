<template lang="pug">
nav.navbar.header.is-fixed-top(role='navigation' aria-label='main navigation')
  .container
    .navbar-brand
      a.navbar-item(href='/')
        strong Design Influences
      .navbar-burger(:class="{ 'is-active': showNav }" @click='showNav = !showNav')
        span(aria-hidden='true')
          span(aria-hidden='true')
            span(aria-hidden='true')
    #main-menu.navbar-menu(:class="{ 'is-active': showNav }")
      .navbar-start
        .navbar-item.has-dropdown.is-hoverable
          a.navbar-link(href='/imagine/') Imagine
          .navbar-dropdown
            a.navbar-item Resources
            a.navbar-item Theory
            a.navbar-item Research
            a.navbar-item Strategy
        .navbar-item.has-dropdown.is-hoverable
          a.navbar-link Design
          .navbar-dropdown
            a.navbar-item Ethics
            a.navbar-item Principles
            a.navbar-item Process
            a.navbar-item Systems
        .navbar-item.has-dropdown.is-hoverable
          a.navbar-link Build
          .navbar-dropdown
            a.navbar-item People
            a.navbar-item Relationships
            a.navbar-item Community
            a.navbar-item Social Architecture
      .navbar-end
        a.navbar-item About
        a.navbar-item Journal
        a.navbar-item Work
        a.navbar-item Resources
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
