<template>
  <div class="page about">
    <hero-section
      title="About"
      subtitle="Putting ideas into practice."
      image="https://source.unsplash.com//ineC_oi7NHs/1600x900"
      image-alt="Perspective Playground"
      color="primary"
      size="is-large"
    />
    <section-intro
      title="Future Literacy"
      subtitle="An orientation to the opportunities afforded by the adjacent possible."
    >
      <p class="intro-paragraph">
        If we are oriented to the past, we may tend to make the same mistakes.
        If we are oriented to the present, we may become resigned to accept the
        way things are. If we are oriented to the future, the possibilities may
        create an indefinite sense of uncertainty, and possibly anxiety, in the
        face of constant change.
      </p>
      <p class="intro-paragraph">
        If we embrace all of reality, we may find the ability to balance memory,
        perception, and expectation to orient ourselves to growth.
      </p>
    </section-intro>
    <section-intro
      title="The Next 100 Years"
      subtitle="Reviving an old idea to reimagine our common life together."
    >
      <p class="intro-paragraph">
        Walter Gropius inaugurated the Bauhaus in Weimar, Germany in 1919 with
        the following words:
      </p>
      <h2>
        The Bauhaus Manifesto
      </h2>
      <h4>
        Art and Technology: A New Unity
      </h4>
      <p>
        The ultimate goal of all art is the building! The ornamentation of the
        building was once the main purpose of the visual arts, and they were
        considered indispensable parts of the great building. Today, they exist
        in complacent isolation, from which they can only be salvaged by the
        purposeful and cooperative endeavours of all artisans. Architects,
        painters and sculptors must learn a new way of seeing and understanding
        the composite character of the building, both as a totality and in terms
        of its parts. Their work will then re-imbue itself with the spirit of
        architecture, which it lost in salon art.
      </p>
      <p>
        The art schools of old were incapable of producing this unity – and how
        could they, for art may not be taught. They must return to the workshop.
        This world of mere drawing and painting of draughtsmen and applied
        artists must at long last become a world that builds. When a young
        person who senses within himself a love for creative endeavour begins
        his career, as in the past, by learning a trade, the unproductive
        'artist' will no longer be condemned to the imperfect practice of art
        because his skill is now preserved in craftsmanship, where he may
        achieve excellence.
      </p>
      <p>
        Architects, sculptors, painters – we all must return to craftsmanship!
        For there is no such thing as ‘art by profession.’ There is no essential
        difference between the artist and the artisan. The artist is an exalted
        artisan. Merciful heaven, in rare moments of illumination beyond man’s
        will, may allow art to blossom from the work of his hand, but the
        foundations of proficiency are indispensable to every artist. This is
        the original source of creative design.
      </p>
      <p>
        So let us therefore create a new guild of craftsmen, free of the
        divisive class pretensions that endeavoured to raise a prideful barrier
        between craftsmen and artists! Let us strive for, conceive and create
        the new building of the future that will unite every discipline,
        architecture and sculpture and painting, and which will one day rise
        heavenwards from the million hands of craftsmen as a clear symbol of a
        new belief to come.
      </p>
    </section-intro>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'AboutPage',
  components: {
    HeroSection,
    SectionIntro
  }
}
</script>
