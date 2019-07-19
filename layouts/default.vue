<template>
  <div id="app">
    <main-nav />
    <nuxt />
    <footer-nav />
  </div>
</template>

<script>
import MainNav from '~/components/MainNav'
import FooterNav from '~/components/FooterNav'

export default {
  components: {
    MainNav,
    FooterNav
  },
  head: {
    htmlAttrs: {
      class: 'has-navbar-fixed-top'
    }
  }
}
</script>
