<template>
  <section id="empresa" :class="[styles.container]">
    <div :class="[styles.wrapper]">
      <img src="@/assets/renee-photo.jpg" alt="Renee Trajar frontal photo" />
      <div :class="[styles.info]">
        <h1>{{ name }}<hr></h1>
        <p>{{ text.aboutFirstPart }}</p>
        <p>{{ text.aboutSecondPart }}</p>
        <p>
          {{ text.aboutCitation }}
          <span :class="[styles.signatureText]">{{ name }}</span>
        </p>
        <button @click="handleClick">{{ callToActionButtonTitle }}</button>
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
      name: 'Renee Trajar',
      callToActionButtonTitle: 'Agende uma visita!',
    };
  },
};
</script>
