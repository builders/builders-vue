<template>
  <section class="hero has-background" :class="['is-' + color, size]">
    <img
      v-if="image"
      class="hero-background is-transparent"
      :src="image"
      :alt="imageAlt"
    />
    <div class="hero-body">
      <div class="container">
        <h1 class="title is-size-2 has-text-weight-bold">
          {{ title }}
        </h1>
        <h3 class="subtitle">
          {{ subtitle }}
        </h3>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroSection',
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
      default: null
    },
    imageAlt: {
      type: String,
      default: null
    },
    color: {
      type: String,
      default: 'primary'
    },
    size: {
      type: String,
      default: 'is-fullheight'
    }
  }
}
</script>

<style lang="scss">
@import '../assets/scss/variables.scss';

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
  img {
    filter: grayscale(1) opacity(0.7);
  }
}
</style>
