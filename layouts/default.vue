<template lang="pug">
  #app
    main-nav
    nuxt
    footer-nav
</template>

<script>
import MainNav from '~/components/MainNav'
import FooterNav from '~/components/FooterNav'

export default {
  components: {
    MainNav,
    FooterNav
  }
}
</script>
