<template lang="pug">
  section.hero.is-fullheight.is-primary.has-background
    img.hero-background.is-transparent(:src="image" :alt="image_alt")
    .hero-body
      .container
        h1.title {{ title }}
        h3.subtitle {{ subtitle }}
</template>

<script>
export default {
  props: {
    title: {
      type: String
    },
    subtitle: {
      type: String
    },
    image: {
      type: String
    },
    image_alt: {
      type: String
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
