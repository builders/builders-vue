<template>
  <section class="section is-medium intro">
    <div class="container">
      <div class="columns is-8">
        <div class="column is-4">
          <div class="content">
            <h1 class="title has-text-weight-bold is-spaced">
              {{ title }}
            </h1>
            <h2 class="subtitle is-size-5 has-text-grey">
              {{ subtitle }}
            </h2>
          </div>
        </div>
        <div class="column is-6 is-offset-2">
          <div class="content">
            <p class="paragraph">
              {{ body }}
            </p>
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
      default: 'Future Literacy'
    },
    subtitle: {
      type: String,
      required: true,
      default:
        'An orientation to the opportunities afforded by the adjacent possible.'
    },
    body: {
      type: String,
      required: true,
      default:
        'If we are oriented to the past, we may tend to make the same mistakes. If we are oriented to the present, we may become resigned to accept the way things are. If we are oriented to the future, the possibilities may create an indefinite sense of uncertainty, and possibly anxiety, in the face of constant change. If we embrace all of reality, we may find the ability to balance memory, perception, and expectation to orient ourselves to growth.'
    }
  }
}
</script>

<style lang="scss">
@media screen and (min-width: 1024px) {
  .intro {
    .subtitle {
      line-height: 1.5em;
      margin-top: 4em;
    }
    .paragraph {
      font-size: 1.5rem;
      line-height: 2em;
    }
  }
}
</style>
