<template>
  <div class="page index">
    <hero-section
      title="Design Influences"
      subtitle="Inspired by the past. Shaping the future."
      image="https://source.unsplash.com/R6cG5_u-Lkw/1600x900"
      image-alt="Bograshov St 1, Tel Aviv-Yafo, Israel"
    />
    <section-intro />
    <section class="section is-medium">
      <div class="container">
        <div class="columns is-variable is-6">
          <icon-card
            title="Imagine"
            icon="triangle"
            color="primary"
            link="/imagine"
          >
            Events
          </icon-card>
          <icon-card
            title="Design"
            icon="circle"
            color="secondary"
            link="/design"
          >
            Workshops
          </icon-card>
          <icon-card title="Build" icon="square" color="tertiary" link="/build">
            Projects
          </icon-card>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import IconCard from '~/components/IconCard'
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'HomePage',

  components: {
    IconCard,
    HeroSection,
    SectionIntro
  }
}
</script>
