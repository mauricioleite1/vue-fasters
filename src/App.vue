<template>
  <the-header></the-header>
  <the-hero></the-hero>
  <about-section></about-section>
  <the-hero></the-hero>
</template>

<script>
import TheHeader from './components/TheHeader/TheHeader.vue';
import TheHero from './components/TheHero/TheHero.vue';
import AboutSection from './components/AboutSection/AboutSection.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheHero,
    AboutSection,
  },
};
</script>

<style lang="scss">
@import "./styles/main";
</style>
