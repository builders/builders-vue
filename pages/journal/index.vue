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
    <section-journal
      title="Articles"
      subtitle="Some thoughts on the influence of design: Inspired by the past. Shaping the future."
      :articles="articles"
    />
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'
import SectionJournal from '~/components/SectionJournal'

import articles from '~/contents/journal/articles.js'

export default {
  name: 'JournalPage',
  components: {
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
