<template lang="pug">
.column
  .card
    header.card-header
      p.card-header-title.has-text-grey
        | {{ title }}
    .card-content
      .content.has-text-centered
        b-icon(:icon='icon' size='is-large' type='is-primary')
    footer.card-footer
      .card-footer-item
        span
          slot
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: true
    }
  }
}
</script>
