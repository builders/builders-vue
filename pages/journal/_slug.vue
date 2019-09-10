<template>
  <div class="article journal">
    <hero-section
      title="Journal"
      subtitle="Progress and the evolution of ideas."
      image="https://source.unsplash.com/CxYHfBkC0vs/1600x900"
      image-alt="Filling a blank page"
      color="secondary"
      size="is-medium"
    />
    <journal-article :attributes="attributes" :html="html" />
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import JournalArticle from '~/components/JournalArticle'

export default {
  name: 'JournalSlug',

  components: {
    HeroSection,
    JournalArticle
  },
  async asyncData({ params, route }) {
    const articleName = params.slug
    const markdownContent = await import(`~/contents/journal/${articleName}.md`)
    return {
      attributes: markdownContent.attributes,
      html: markdownContent.html,
      currentUrl: route.path
    };
  }
};
</script>
