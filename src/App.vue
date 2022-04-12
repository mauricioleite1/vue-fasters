<template>
  <the-header></the-header>
  <the-hero></the-hero>
  <about-section></about-section>
  <highlighted-comment></highlighted-comment>
  <the-hero></the-hero>
</template>

<script>
import TheHeader from './components/TheHeader/TheHeader.vue';
import TheHero from './components/TheHero/TheHero.vue';
import AboutSection from './components/AboutSection/AboutSection.vue';
import HighlightedComment from './components/HighlightedComment/HighlightedComment.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheHero,
    AboutSection,
    HighlightedComment,
  },
};
</script>

<style lang="scss">
@import "./styles/main";
</style>
