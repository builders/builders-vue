<template lang="pug">
nav.navbar.header.is-fixed-top(role='navigation' aria-label='main navigation')
  .container
    .navbar-brand
      n-link.navbar-item(to='/')
        strong Design Influences
      .navbar-burger(:class="{ 'is-active': showNav }" @click='showNav = !showNav')
        span(aria-hidden='true')
        span(aria-hidden='true')
        span(aria-hidden='true')
    #main-menu.navbar-menu(:class="{ 'is-active': showNav }")
      .navbar-start
        .navbar-item.has-dropdown.is-hoverable.menu-imagine
          n-link.navbar-link(to='/imagine') Imagine
          .navbar-dropdown
            a.navbar-item Resources
            a.navbar-item Theory
            a.navbar-item Research
            a.navbar-item Strategy
        .navbar-item.has-dropdown.is-hoverable.menu-design
          n-link.navbar-link(to='/design') Design
          .navbar-dropdown
            a.navbar-item Ethics
            a.navbar-item Principles
            a.navbar-item Process
            a.navbar-item Systems
        .navbar-item.has-dropdown.is-hoverable.menu-build
          n-link.navbar-link(to='/build') Build
          .navbar-dropdown
            a.navbar-item People
            a.navbar-item Relationships
            a.navbar-item Community
            a.navbar-item Social Architecture
      .navbar-end
        a.navbar-item About
        a.navbar-item Journal
        a.navbar-item Work
        a.navbar-item Resources
</template>

<script>
export default {
  name: 'MainNav',
  data() {
    return {
      showNav: false
    }
  }
}
</script>

<style lang="scss">
@import '../assets/css/variables.scss';

.menu-imagine {
  &.navbar-item.has-dropdown:hover {
    .navbar-link {
      background-color: $primary;
      color: #fff;
      &:not(.is-arrowless)::after {
        border-color: #fff;
      }
    }
  }
  .navbar-link {
    &:hover {
      color: #fff;
    }
    &:not(.is-arrowless)::after {
      border-color: $primary;
    }
  }
}

.menu-design {
  &.navbar-item.has-dropdown:hover {
    .navbar-link {
      background-color: $secondary;
      color: #fff;
      &:not(.is-arrowless)::after {
        border-color: #fff;
      }
    }
  }
  .navbar-link {
    &:hover {
      color: #fff;
    }
    &:not(.is-arrowless)::after {
      border-color: $secondary;
    }
  }
}

.menu-build {
  &.navbar-item.has-dropdown:hover {
    .navbar-link {
      background-color: $tertiary;
      color: #fff;
      &:not(.is-arrowless)::after {
        border-color: #fff;
      }
    }
  }
  .navbar-link {
    &:hover {
      color: #fff;
    }
    &:not(.is-arrowless)::after {
      border-color: $tertiary;
    }
  }
}

@media screen and (min-width: 1024px) {
  .menu-imagine {
    .navbar-dropdown {
      a.navbar-item {
        &:hover {
          background-color: $primary;
          color: #fff;
        }
      }
    }
  }
  .menu-design {
    .navbar-dropdown {
      a.navbar-item {
        &:hover {
          background-color: $secondary;
          color: #fff;
        }
      }
    }
  }
  .menu-build {
    .navbar-dropdown {
      a.navbar-item {
        &:hover {
          background-color: $tertiary;
          color: #fff;
        }
      }
    }
  }
}
</style>
