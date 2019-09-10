<template>
  <section class="section section-article is-medium">
    <div class="container">
      <div class="columns is-8">
        <div class="column is-4">
          <div class="content">
            <h2 class="title is-size-3 has-text-weight-bold is-spaced">
              {{ attributes.title }}
            </h2>
            <h3 class="subtitle is-size-5 has-text-grey">
              {{ attributes.subtitle }}
            </h3>
            <p class="date">
              {{ attributes.date }}
            </p>
          </div>
        </div>
        <div class="column is-6 is-offset-2">
          <div class="content body">
            <span v-html="html" class="markdown"></span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'JournalArticle',
  props: {
    attributes: {
      type: Object,
      required: true,
      default: {}
    },
    html: {
      type: Object,
      required: true,
      default: {}
    }
  }
}
</script>

<style lang="scss">
@media screen and (min-width: 1024px) {
  .section-article {
    .subtitle {
      line-height: 1.5em;
      margin-top: 4em;
    }
  }
}
</style>
