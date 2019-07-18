<template>
  <div class="page about">
    <hero-section
      title="About"
      subtitle="Putting ideas into practice."
      image="https://source.unsplash.com//ineC_oi7NHs/1600x900"
      image-alt="Perspective Playground"
      color="primary"
    >
      <div class="container"></div>
    </hero-section>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'

export default {
  name: 'AboutPage',
  components: {
    HeroSection
  }
}
</script>
