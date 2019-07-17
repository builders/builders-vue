<template lang="pug">
  section.hero.is-fullheight.is-primary.has-background
    img.hero-background.is-transparent(:src='image' :alt='imageAlt')
    .hero-body
      .container
        h1.title {{ title }}
        h3.subtitle {{ subtitle }}
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Design Influences'
    },
    subtitle: {
      type: String,
      default: 'Inspired by the past. Shaping the future.'
    },
    image: {
      type: String,
      default: 'https://source.unsplash.com/nBWmOsOdi4Y/1600x900'
    },
    imageAlt: {
      type: String,
      default: 'Bauhaus Archive, Berlin'
    }
  }
}
</script>

<style lang="stylus">
.hero
  &.has-background
    position: relative
    overflow: hidden
  &-background
    position: absolute
    object-fit: cover
    object-position: center center
    width: 100%
    height: 100%
    &.is-transparent
      opacity: 0.3
</style>
