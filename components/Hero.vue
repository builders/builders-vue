<template lang="pug">
  section.hero.is-fullheight.has-background(:class='backgroundClass')
    img.hero-background.is-transparent(:src='image' :alt='imageAlt')
    .hero-body
      .container
        h1.title {{ title }}
        h3.subtitle {{ subtitle }}
</template>

<script>
export default {
  name: 'Hero',
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
    },
    backgroundClass: {
      type: String,
      default: 'is-primary'
    }
  }
}
</script>

<style lang="scss">
@import '../assets/css/variables.scss';

.hero {
  &.has-background {
    position: relative;
    overflow: hidden;
  }
  &-background {
    position: absolute;
    object-fit: cover;
    object-position: center center;
    width: 100%;
    height: 100%;
    &.is-transparent {
      opacity: 0.3;
    }
  }
  &.is-secondary {
    background-color: $secondary;
    color: #fff;
    .title,
    .subtitle {
      color: #fff;
    }
  }
  &.is-tertiary {
    background-color: $tertiary;
    color: #fff;
    .title,
    .subtitle {
      color: #fff;
    }
  }
}
</style>
