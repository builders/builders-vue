<template>
  <div class="page index">
    <hero-section
      title="Design Influences"
      subtitle="Inspired by the past. Shaping the future."
      image="/images/tel-aviv-yafo-israel-R6cG5_u-Lkw.jpg"
      image-alt="Bograshov St 1, Tel Aviv-Yafo, Israel"
    />
    <section-intro
      title="A New Synthesis"
      subtitle="The past century has been marked by division. We need a new synthesis."
    >
      <p class="intro-paragraph">
        In the service of industrial models of social and political engineering,
        art and technology have been co-opted to participate in a
        military-industrial complex that is a synthesis of our worst human
        characteristics: greed and hatred.
      </p>
      <p class="intro-paragraph">
        We are caught in a dialectic of opposing forces, in the politics of
        thesis and antithesis, right versus left. We need a new synthesis that
        transcends the old paradigms. Unity in diversity is the model for both
        the organism and the planet.
      </p>
      <p class="intro-paragraph">
        <strong>The new synthesis is integrating biology and physics.</strong>
        The future of design and architecture may be in the integration of the
        separate disciplines to learn how interconnected systems work and model
        the built environment to imitate the processes of living organisms. We
        are beginning to see these changes happening through the self-organizing
        principles of biological adaptation.
      </p>
    </section-intro>
    <section-journal
      title="Journal"
      subtitle="Progress and the evolution of ideas."
      :articles="articles"
    />
    <section class="section is-medium">
      <div class="container">
        <div class="columns is-variable is-6">
          <icon-card
            title="Imagine"
            icon="circle"
            color="primary"
            link="/imagine"
          >
            Events
          </icon-card>
          <icon-card
            title="Design"
            icon="triangle"
            color="secondary"
            link="/design"
          >
            Workshops
          </icon-card>
          <icon-card
            title="Build"
            icon="square"
            color="tertiary"
            link="/build">
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
import SectionJournal from '~/components/SectionJournal'

import articles from '~/contents/journal/articles.js'

export default {
  name: 'HomePage',

  components: {
    IconCard,
    HeroSection,
    SectionIntro,
    SectionJournal
  },
  async asyncData ({ route }) {
    const promises = articles.map(article => import(`~/contents/journal/${article}.md`))
    return { articles: await Promise.all(promises) }
  }
}
</script>
