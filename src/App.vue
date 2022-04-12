<template>
  <the-header></the-header>
  <the-hero></the-hero>
</template>

<script>
import TheHeader from './components/TheHeader/TheHeader.vue';
import TheHero from './components/TheHero/TheHero.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheHero,
  },
};
</script>

<style lang="scss">
@import "./styles/main";
</style>
