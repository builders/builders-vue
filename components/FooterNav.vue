<template>
  <footer class="footer footer-nav">
    <div class="container">
      <div class="columns">
        <div class="column is-3">
          <div class="footer-link-title site-name">
            <n-link to="/">
              Design Influences
            </n-link>
          </div>
        </div>
        <div class="column is-3 menu-imagine">
          <h3 class="footer-link-title">
            <n-link to="/imagine">
              Imagine
            </n-link>
          </h3>
          <div class="footer-links">
            <div class="footer-link">
              <a>
                Resources
              </a>
            </div>
            <div class="footer-link">
              <a>
                Theory
              </a>
            </div>
            <div class="footer-link">
              <a>
                Research
              </a>
            </div>
            <div class="footer-link">
              <a>
                Strategy
              </a>
            </div>
          </div>
        </div>
        <div class="column is-3 menu-design">
          <h3 class="footer-link-title">
            <n-link to="/design">
              Design
            </n-link>
          </h3>
          <div class="footer-links">
            <div class="footer-link">
              <a>
                Ethics
              </a>
            </div>
            <div class="footer-link">
              <a>
                Principles
              </a>
            </div>
            <div class="footer-link">
              <a>
                Process
              </a>
            </div>
            <div class="footer-link">
              <a>
                Systems
              </a>
            </div>
          </div>
        </div>
        <div class="column is-3 menu-build">
          <h3 class="footer-link-title">
            <n-link to="/build">
              Build
            </n-link>
          </h3>
          <div class="footer-links">
            <div class="footer-link">
              <a>
                People
              </a>
            </div>
            <div class="footer-link">
              <a>
                Relationships
              </a>
            </div>
            <div class="footer-link">
              <a>
                Community
              </a>
            </div>
            <div class="footer-link">
              <a>
                Social Architecture
              </a>
            </div>
          </div>
        </div>
      </div>
      <div class="siteinfo">
        <div class="social-media">
          <a class="medium" href="https://medium.com/builderscollective">
            <img class="icon" src="/images/medium.svg" alt="Medium" />
          </a>
          <a class="twitter" href="https://twitter.com/bldrsco">
            <img class="icon" src="/images/twitter-square.svg" alt="Twitter" />
          </a>
          <a class="facebook" href="https://www.facebook.com/bldrscollective">
            <img class="icon" src="/images/facebook-square.svg" alt="Facebook" />
          </a>
          <a class="instagram" href="https://www.instagram.com/bldrsco">
            <img class="icon" src="/images/instagram.svg" alt="Instagram" />
          </a>
        </div>
        <p class="credit">
          A project of the&nbsp;
          <a href="https://builderscollective.com">
            builders collective
          </a>
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterNav'
}
</script>

<style lang="scss">
@import '../assets/css/variables.scss';

.footer-nav {
  background: #333;
  color: #fff;
  a {
    color: #999;
    &:hover {
      color: #00aeef;
    }
  }
  .menu-design {
    a:hover {
      color: $secondary;
    }
  }
  .menu-build {
    a:hover {
      color: $tertiary;
    }
  }
}

.footer-link-title {
  font-size: 1.3rem;
  margin-bottom: 1rem;
  a {
    color: #fff;
    display: block;
  }
}

.footer-link {
  a {
    display: block;
    padding-top: 0.25em;
    padding-bottom: 0.25em;
  }
}

.siteinfo {
  font-size: 0.9rem;
  color: #666;
  border-top: 1px solid #444;
  margin-top: 3rem;
  padding-top: 2rem;
  .social-media {
    margin-bottom: 1rem;
    a {
      margin-right: 1rem;
      color: #666;
      .icon {
        height: 30px;
        width: 30px;
        font-size: 30px;
        .mdi:before {
          font-size: 30px;
        }
      }
      &:hover {
        color: #00aeef;
      }
    }
  }
}

@media screen and (min-width: 768px) {
  .siteinfo {
    .social-media {
      float: right;
      a {
        margin-left: 1rem;
        margin-right: 0;
      }
    }
    p.credit {
      margin-top: 0.3rem;
    }
  }
}
</style>
