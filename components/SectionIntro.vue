<template>
  <section class="section section-intro is-medium">
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
            <slot />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'SectionIntro',
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
    }
  }
}
</script>

<style lang="scss">
@media screen and (min-width: 1024px) {
  .section-intro {
    .subtitle {
      line-height: 1.5em;
      margin-top: 4em;
    }
    .body {
      p.intro-paragraph {
        font-size: 1.4rem;
        line-height: 2em;
        margin-bottom: 2em;
      }
    }
  }
}
</style>
