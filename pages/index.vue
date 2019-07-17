<template>
  <div class="index">
    <hero />
    <div class="container">
      <section class="section">
        <div class="columns is-mobile">
          <card title="Imagine" icon="triangle">
            Events
          </card>

          <card title="Design" icon="circle">
            Workshops
          </card>

          <card title="Build" icon="square">
            Projects
          </card>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import Card from '~/components/Card'
import Hero from '~/components/Hero'

export default {
  name: 'HomePage',

  components: {
    Card,
    Hero
  }
}
</script>
