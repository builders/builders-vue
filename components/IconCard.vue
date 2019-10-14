<template>
  <div class="column">
    <div class="card">
      <header class="card-header">
        <p class="card-header-title has-text-grey">
          {{ title }}
        </p>
      </header>
      <div class="card-content">
        <div class="content has-text-centered">
          <n-link :to="link">
            <img :src="image" :alt="title" />
          </n-link>
        </div>
      </div>
      <footer class="card-footer">
        <div class="card-footer-item">
          <span>
            <slot />
          </span>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IconCard',
  props: {
    title: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    },
    color: {
      type: String,
      required: true,
      default: 'primary'
    },
    link: {
      type: String,
      required: true
    }
  }
}
</script>

<style>
.icon.is-large {
  height: 10rem;
  width: 10rem;
}
.mdi-48px.mdi:before {
  font-size: 10rem;
}
</style>
