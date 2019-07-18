<template lang="pug">
.page.design
  hero-section(title='Design' subtitle='Improving the experience of all living things on Earth.' image='https://source.unsplash.com/nrhnluxL1E8/1600x900' image-alt='Bauhaus Archive, Berlin' background-class='is-secondary')
    .container
</template>

<script>
import HeroSection from '~/components/HeroSection'

export default {
  name: 'DesignPage',
  components: {
    HeroSection
  }
}
</script>
