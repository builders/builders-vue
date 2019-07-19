<template>
  <div class="page work">
    <hero-section
      title="Work"
      subtitle="Finding flow in the search for agency, purpose, and mastery."
      image="https://source.unsplash.com/8KfCR12oeUM/1600x900"
      image-alt="In the line of fire"
      color="tertiary"
      size="is-large"
    />
    <section-intro
      title="Ecological Literacy"
      subtitle="Recognizing that we are living organisms who are part of the living system of the Earth."
    >
      <p class="intro-paragraph">
        The built environment is the physical infrastructure that contains and
        directs our social and economic relationships in patterns designed
        before we became aware of more effective and beneficial alternatives and
        opportunities, or the toxic effects of our legacy structures.
      </p>
      <p>
        If the economic system that we have designed better serves its own
        purpose of perpetual economic growth, it may no longer be serving the
        human needs it was designed to serve. Does the machine serve us or do we
        serve the machine?
      </p>
      <p>
        We have together built a machine into a form that reflects the
        fragmented and siloed intellectual disciplines that we model after
        educational institutions, corporate organizational structures, and
        political systems that divide our thinking and work into discrete
        categories and disciplines.
      </p>
      <p>
        Diversity has become our greatest asset but our politics, our economics,
        and our built environment favour homogeneity and separation. The
        tendency of the system we have designed toward homogeneity is destroying
        the delicate balance of the earth’s diverse ecosystem.
      </p>
      <p>
        <strong>
          Biology provides the model for a sustainable future. The symbiotic
          relationships of the various organisms that form our own bodies are a
          model of systems that have been proven to survive and thrive on earth.
        </strong>
      </p>
    </section-intro>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'WorkPage',
  components: {
    HeroSection,
    SectionIntro
  }
}
</script>
