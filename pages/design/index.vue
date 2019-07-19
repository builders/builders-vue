<template>
  <div class="page design">
    <hero-section
      title="Design"
      subtitle="Improving the experience of all living things on Earth."
      image="https://source.unsplash.com/nrhnluxL1E8/1600x900"
      image-alt="Bauhaus Archive, Berlin"
      color="secondary"
    />
    <section-intro
      title="Living Systems"
      subtitle="The challenge of our century: how might we model social systems after living organisms?"
    >
      <p class="intro-paragraph">
        Design is evolving from physical artifacts to human experience:
        perception (senses), cognition (mind), emotion (heart), and action
        (body). The future of design and architecture may be in the integration
        of the separate disciplines to learn how interconnected systems work and
        model the built environment to imitate the processes of living
        organisms.
      </p>
    </section-intro>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'DesignPage',
  components: {
    HeroSection,
    SectionIntro
  }
}
</script>
