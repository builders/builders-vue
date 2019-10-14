<template>
  <div class="page imagine">
    <hero-section
      title="Imagine"
      subtitle="Creativity and innovation at the intersection of art and science."
      image="/images/bauhaus-archiv-berlin-nBWmOsOdi4Y.jpg"
      image-alt="Bauhaus Archive, Berlin"
      color="primary"
    />
    <section-intro
      title="The Power of Imagination"
      subtitle="The big picture thinking that we need to solve the greatest challenges that we are facing at this moment in time."
    >
      <p class="intro-paragraph">
        There is a terrible misconception in school that when we take art that
        we are teaching people to draw. What we are really doing is teaching
        people to see. That’s the important function. That’s why I think it is
        tragic when school funding gets cut, they cut out the art. To be
        creative, we must choose something that is really hard, that we might
        fail at, and have failed at; then we’re more likely to come up with
        something that is fresh and different.
      </p>
    </section-intro>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'ImaginePage',
  components: {
    HeroSection,
    SectionIntro
  }
}
</script>
