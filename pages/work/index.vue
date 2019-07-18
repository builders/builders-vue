<template>
  <div class="page work">
    <hero-section
      title="Work"
      subtitle="Finding flow in the search for agency, purpose, and mastery."
      image="https://source.unsplash.com/8KfCR12oeUM/1600x900"
      image-alt="In the line of fire"
      color="primary"
    >
      <div class="container"></div>
    </hero-section>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'

export default {
  name: 'WorkPage',
  components: {
    HeroSection
  }
}
</script>
