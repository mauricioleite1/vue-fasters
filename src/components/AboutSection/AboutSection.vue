<template>
  <section :class="[styles.container]">
    <div :class="[styles.wrapper]">
      <img src="@/assets/renee-photo.jpg" alt="Renee Trajar frontal photo" />
      <div :class="[styles.info]">
        <h1>Renee Trajar<hr></h1>
        <p>{{ text.aboutFirstPart }}</p>
        <p>{{ text.aboutSecondPart }}</p>
        <p>{{ text.aboutCitation }}</p>
      </div>
    </div>
  </section>
</template>

<script>
import styles from './AboutSection.module.scss';
import text from '../../utils/data';

export default {
  name: 'AboutSection',
  data() {
    return {
      styles,
      text,
    };
  },
};
</script>
