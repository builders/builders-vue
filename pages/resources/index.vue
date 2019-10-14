<template>
  <div class="page resources">
    <hero-section
      title="Resources"
      subtitle="Making sense through empathy, curiosity, and research."
      image="/images/stadsbiblioteket-stockholm-2JIvboGLeho.jpg"
      image-alt="Stadsbiblioteket, Stockholm, Sweden"
      color="primary"
      size="is-large"
    />
    <section-intro
      title="Media Literacy"
      subtitle="Editorial in the age of information overload and information overlords."
    >
      <p class="intro-paragraph">
        In the age of mass media, there was power in the role of the editors as
        the gatekeepers of information and the arbiters of salience, taste, and
        social propriety. The digital age has democratized access to the tools
        of production, but it has also centralized resources, wealth, and power
        in large corporate monopolies.
      </p>
    </section-intro>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'ResourcesPage',
  components: {
    HeroSection,
    SectionIntro
  }
}
</script>
