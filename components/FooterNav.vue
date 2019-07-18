<template lang="pug">
  footer.footer.footer-nav
    .container
      .columns
        .column.is-3
          .footer-link-title.site-name
            n-link(to='/')
              | Design Influences
        .column.is-3.menu-imagine
          h3.footer-link-title
            n-link(to="/imagine")
              | Imagine
          .footer-links
            .footer-link
              a Resources
            .footer-link
              a Theory
            .footer-link
              a Research
            .footer-link
              a Strategy
        .column.is-3.menu-design
          h3.footer-link-title
            n-link(to="/design")
              | Design
          .footer-links
            .footer-link
              a Ethics
            .footer-link
              a Principles
            .footer-link
              a Process
            .footer-link
              a Systems
        .column.is-3.menu-build
          h3.footer-link-title
            n-link(to="/build")
              | Build
          .footer-links
            .footer-link
              a People
            .footer-link
              a Relationships
            .footer-link
              a Community
            .footer-link
              a Social Architecture
      .siteinfo
        .social-media
          a.medium(href="https://medium.com/builderscollective")
            b-icon(icon='medium')
          a.twitter(href="https://twitter.com/bldrsco")
            b-icon(icon='twitter-box')
          a.facebook(href="https://www.facebook.com/bldrscollective")
            b-icon(icon='facebook-box')
          a.instagram(href="https://www.instagram.com/bldrsco")
            b-icon(icon='instagram')
        p.credit A project of the&nbsp;
          a(href='https://builderscollective.com') builders collective
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
