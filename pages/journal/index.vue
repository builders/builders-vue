<template>
  <div class="page journal">
    <hero-section
      title="Journal"
      subtitle="Progress and the evolution of ideas."
      image="https://source.unsplash.com/CxYHfBkC0vs/1600x900"
      image-alt="Filling a blank page"
      color="secondary"
      size="is-large"
    />
    <section-intro
      title="Cultural Literacy"
      subtitle="Navigating the social, political, and economic landscape of cultural identity."
    >
      <p class="intro-paragraph">
        Finding our way in the world is wrapped up in issues of identity that
        are intimately connected to our position in the social, political, and
        economic hierarchies in which we are situated culturally,
        geographically, and intellectually. It is the water in which we live and
        the air we breathe. We benefit from the privileges we inhabit or we are
        marginalized by the unspoken sanctions of our social status.
      </p>
    </section-intro>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'JournalPage',
  components: {
    HeroSection,
    SectionIntro
  }
}
</script>
