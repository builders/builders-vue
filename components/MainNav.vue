<template>
  <nav
    class="navbar header is-fixed-top"
    role="navigation"
    aria-label="main navigation"
  >
    <div class="container">
      <div class="navbar-brand">
        <n-link class="navbar-item" to="/">
          <strong>
            Design Influences
          </strong>
        </n-link>
        <div
          class="navbar-burger"
          :class="{ 'is-active': showNav }"
          @click="showNav = !showNav"
        >
          <span aria-hidden="true" />
          <span aria-hidden="true" />
          <span aria-hidden="true" />
        </div>
      </div>
      <div class="navbar-menu" id="main-menu" :class="{ 'is-active': showNav }">
        <div class="navbar-start">
          <div class="navbar-item has-dropdown is-hoverable menu-imagine">
            <n-link class="navbar-link" to="/imagine">
              Imagine
            </n-link>
            <div class="navbar-dropdown">
              <a class="navbar-item">Resources</a>
              <a class="navbar-item">Theory</a>
              <a class="navbar-item">Research</a>
              <a class="navbar-item">Strategy</a>
            </div>
          </div>
          <div class="navbar-item has-dropdown is-hoverable menu-design">
            <n-link class="navbar-link" to="/design">
              Design
            </n-link>
            <div class="navbar-dropdown">
              <a class="navbar-item">Ethics</a>
              <a class="navbar-item">Principles</a>
              <a class="navbar-item">Process</a>
              <a class="navbar-item">Systems</a>
            </div>
          </div>
          <div class="navbar-item has-dropdown is-hoverable menu-build">
            <n-link class="navbar-link" to="/build">
              Build
            </n-link>
            <div class="navbar-dropdown">
              <a class="navbar-item">People</a>
              <a class="navbar-item">Relationships</a>
              <a class="navbar-item">Community</a>
              <a class="navbar-item">Social Architecture</a>
            </div>
          </div>
        </div>
        <div class="navbar-end">
          <n-link class="navbar-item" to="/about">
            About
          </n-link>
          <n-link class="navbar-item" to="/journal">
            Journal
          </n-link>
          <n-link class="navbar-item" to="/work">
            Work
          </n-link>
          <n-link class="navbar-item" to="/resources">
            Resources
          </n-link>
        </div>
      </div>
    </div>
  </nav>
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

.navbar-item.is-hoverable:focus .navbar-dropdown,
.navbar-item.is-hoverable:focus-within .navbar-dropdown {
  display: none;
}
.navbar-item.is-hoverable:hover .navbar-dropdown {
  display: block;
}

.menu-design .nuxt-link-active {
  color: $secondary;
}
.menu-build .nuxt-link-active {
  color: $tertiary;
}
a.navbar-link:focus-within,
a.navbar-item:hover,
a.navbar-item:focus,
a.navbar-item.nuxt-link-active {
  background-color: transparent;
}
</style>
