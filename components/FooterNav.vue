<template lang="pug">
  footer.footer.footer-nav
    .container
      .columns
        .column.is-3
          .footer-link-title.site-name
            a(href='/')
              | Design Influences
        .column.is-3
          h3.footer-link-title
            a(href="/imagine/")
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
        .column.is-3
          h3.footer-link-title
            a(href="/design/")
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
        .column.is-3
          h3.footer-link-title
            a(href="/build/")
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
      .social-media
        a.instagram
          i.fab.fa-instagram
      p.siteinfo Site design by Stephen Bau, Builders Collective
</template>

<style lang="stylus">
.footer-nav
  background: #333
  color: #fff
.footer-link-title
  font-size: 1.3rem
  margin-bottom: 1rem
  a
    color: #fff
    display: block
    &:hover
      color: #00aeef
.footer-link
  a
    color: #999
    display: block
    padding-top: 0.25em
    padding-bottom: 0.25em
    &:hover
      color: #00aeef
.siteinfo
  font-size: 0.9rem;
  color: #666
  border-top: 1px solid #444
  margin-top: 3rem;
  padding-top: 2rem;
</style>
