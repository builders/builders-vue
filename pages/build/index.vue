<template>
  <div class="page build">
    <hero-section
      title="Build"
      subtitle="Building resilience, relationships, and community."
      image="/images/bauhaus-building-dessau-JUHbj2ZV5hE.jpg"
      image-alt="Bauhaus Building, Dessau"
      color="tertiary"
    />
    <section-intro
      title="Social Architecture"
      subtitle="From the design of physical artifacts to the synthesis of physics and biology in the formation of living systems."
    >
      <p class="intro-paragraph">
        Design goes beyond the pragmatic application of visual style to cultural
        artifacts. In other words, design is more than making things look
        pretty. It is a way of thinking and a process of working that enhances
        the ability of an individual or group of individuals to build
        relationships with the people in their community, locally and globally,
        and to realize their vision to meet needs, solve problems, and overcome
        challenges, not by fighting the existing reality, but by creating new
        models of reality to make the old ones obsolete.
      </p>
    </section-intro>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'BuildPage',
  components: {
    HeroSection,
    SectionIntro
  }
}
</script>
