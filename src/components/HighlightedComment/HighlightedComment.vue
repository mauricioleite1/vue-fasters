<template>
  <section :class="[styles.container]">
    <div :class="[styles.wrapper]">
      <div :class="[styles.text]">
        <p>{{ text.highlight }}</p>
        <div>
          <h3>Nelson Garey</h3>
          <h4>Advogado | Nelson Garey Advogados Associados</h4>
        </div>
      </div>
      <img :class="[styles.photo]" src="@/assets/highlighted-comment-1.png" alt="" />
      <img :class="[styles.bgPhoto]" src="@/assets/highlighted-comment-2.jpg" alt="" />
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
    };
  },
};
</script>
