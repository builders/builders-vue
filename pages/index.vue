<template>
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
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',

  components: {
    Card
  }
}
</script>
