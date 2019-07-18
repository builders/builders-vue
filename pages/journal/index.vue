<template>
  <div class="page journal">
    <hero-section
      title="Journal"
      subtitle="Progress and the evolution of ideas."
      image="https://source.unsplash.com/CxYHfBkC0vs/1600x900"
      image-alt="Filling a blank page"
      color="primary"
    >
      <div class="container"></div>
    </hero-section>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'

export default {
  name: 'JournalPage',
  components: {
    HeroSection
  }
}
</script>
