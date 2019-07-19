<template>
  <div class="page index">
    <hero-section
      title="Design Influences"
      subtitle="Inspired by the past. Shaping the future."
      image="https://source.unsplash.com/R6cG5_u-Lkw/1600x900"
      image-alt="Bograshov St 1, Tel Aviv-Yafo, Israel"
    />
    <section-intro
      title="Future Literacy"
      subtitle="An orientation to the opportunities afforded by the adjacent possible."
    >
      <p>
        If we are oriented to the past, we may tend to make the same mistakes.
        If we are oriented to the present, we may become resigned to accept the
        way things are. If we are oriented to the future, the possibilities may
        create an indefinite sense of uncertainty, and possibly anxiety, in the
        face of constant change.
      </p>
      <p>
        If we embrace all of reality, we may find the ability to balance memory,
        perception, and expectation to orient ourselves to growth.
      </p>
    </section-intro>
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
