<template>
  <section class="section section-journal is-medium">
    <div class="container">
      <div class="columns is-8">
        <div class="column is-4">
          <div class="content">
            <h2 class="title is-size-3 has-text-weight-bold is-spaced">
              {{ title }}
            </h2>
            <h3 class="subtitle is-size-5 has-text-grey">
              {{ subtitle }}
            </h3>
          </div>
        </div>
        <div class="column is-6 is-offset-2">
          <div class="content body">
            <article class="post content" v-for="(article, index) in articles" :key="index">
              <div class="post-aside">
                <p class="post-meta"><small>{{ article.attributes.date }}</small></p>
                <h3 class="post-title"><nuxt-link :to="article.attributes.link">{{ article.attributes.title }}</nuxt-link></h3>
                <p class="post-description">{{ article.attributes.description }}</p>
              </div>
            </article>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'SectionJournal',
  props: {
    title: {
      type: String,
      required: true,
      default: 'Title'
    },
    subtitle: {
      type: String,
      required: true,
      default: 'Subtitle'
    },
    articles: {
      type: Array,
      required: true,
      default: []
    }
  }
}
</script>

<style lang="scss">
@media screen and (min-width: 1024px) {
  .section-journal {
    .subtitle {
      line-height: 1.5em;
      margin-top: 4em;
    }
  }
}

.section-journal {
  .post {
    border-top: 1px solid #ddd;
    padding: 0.5rem 0 3rem;
    margin-bottom: 0;

    &:last-child {
      border-bottom: 1px solid #ddd;
    }

    .post-meta {
      font-size: 0.9rem;
      color: #aaa;
      text-transform: uppercase;
      letter-spacing: 0.1em;
    }
    .post-title {
      margin-top: 1.5rem;
    }
  }
}
</style>
