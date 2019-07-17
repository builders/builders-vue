<template lang="pug">
.page.index
  hero(title='Design Influences' subtitle='Inspired by the past. Shaping the future.' image='https://source.unsplash.com/R6cG5_u-Lkw/1600x900' image-alt='Bograshov St 1, Tel Aviv-Yafo, Israel')
    .container
      section.section
        .columns.is-mobile
          card(title='Imagine' icon='triangle')
            | Events
          card(title='Design' icon='circle')
            | Workshops
          card(title='Build' icon='square')
            | Projects
</template>

<script>
import Card from '~/components/Card'
import Hero from '~/components/Hero'

export default {
  name: 'HomePage',

  components: {
    Card,
    Hero
  }
}
</script>
