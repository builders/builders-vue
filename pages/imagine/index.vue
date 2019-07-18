<template lang="pug">
.page.imagine
  hero-section(title='Imagine' subtitle='Creativity and innovation at the intersection of art and science.' image='https://source.unsplash.com/nBWmOsOdi4Y/1600x900' image-alt='Bauhaus Archive, Berlin')
    .container
</template>

<script>
import HeroSection from '~/components/HeroSection'

export default {
  name: 'ImaginePage',
  components: {
    HeroSection
  }
}
</script>
