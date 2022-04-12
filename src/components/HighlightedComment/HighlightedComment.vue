<template>
  <section :class="[styles.container]">
    Highlight
    <img src="@/assets/highlighted-comment-1.png" alt="" />
  </section>
</template>

<script>
import styles from './HighlightedComment.module.scss';

export default {
  name: 'HighlightedComment',
  data() {
    return {
      styles,
    };
  },
};
</script>
