<template>
  <section :class="[styles.container]">
    <div :class="[styles.wrapper]">
      <div :class="[styles.text]">
        <p>{{ text.highlight }}</p>
        <div>
          <h3>{{ name }}</h3>
          <h4>{{ title }}</h4>
        </div>
      </div>
      <img :class="[styles.photo]" src="@/assets/highlighted-comment-1.png" alt="Nelson Garey" />
      <img
        :class="[styles.bgPhoto]"
        src="@/assets/highlighted-comment-2.jpg"
        alt="Nelson Garey in background"
      />
    </div>
  </section>
</template>

<script>
import text from '@/utils/data';
import styles from './HighlightedComment.module.scss';

export default {
  name: 'HighlightedComment',
  data() {
    return {
      styles,
      text,
      name: 'Nelson Garey',
      title: 'Advogado | Nelson Garey Advogados Associados',
    };
  },
};
</script>
