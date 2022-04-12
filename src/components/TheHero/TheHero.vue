<template>
  <div :class="[styles.container]">Hero</div>
</template>

<script>
import styles from './TheHero.module.scss';

export default {
  name: 'TheHero',
  data() {
    return {
      styles,
    };
  },
};
</script>
