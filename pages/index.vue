<template lang="pug">
.page.index
  hero-section(title='Design Influences' subtitle='Inspired by the past. Shaping the future.' image='https://source.unsplash.com/R6cG5_u-Lkw/1600x900' image-alt='Bograshov St 1, Tel Aviv-Yafo, Israel')
  .container
    section.section
      .columns.is-mobile
        icon-card(title='Imagine' icon='triangle')
          | Events
        icon-card(title='Design' icon='circle')
          | Workshops
        icon-card(title='Build' icon='square')
          | Projects
</template>

<script>
import IconCard from '~/components/IconCard'
import HeroSection from '~/components/HeroSection'

export default {
  name: 'HomePage',

  components: {
    IconCard,
    HeroSection
  }
}
</script>
