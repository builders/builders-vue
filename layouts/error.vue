<template>
  <div class="page error">
    <hero-section
      :title="error.statusCode === 404 ? 'Page not found' : 'An error occurred'"
      subtitle="Oops! Something went wrong."
      color="tertiary"
      size="is-large"
    />
    <section-intro
      title="Keep looking"
      subtitle="If you still haven’t found what you’re looking for, we’re here to help as best as we can."
    >
      <p class="intro-paragraph">
        Isn’t the search a life-long quest to discover meaning, purpose, and
        belonging? We hope to point you in the right direction, but there are
        limits to what we can do. For what you are looking for, you may simply
        be in the wrong place.
      </p>
    </section-intro>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'ErrorPage',
  components: {
    HeroSection,
    SectionIntro
  },
  props: {
    error: {
      type: Object,
      default: () => {}
    }
  }
}
</script>
