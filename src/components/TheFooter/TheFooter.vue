<template>
  <footer :class="[styles.container]">
    <div :class="[styles.wrapper]">
      <div :class="[styles.leftContent]">
        <img src="@/assets/footer-logo.svg" alt="Renee Trajar Logo" />
        <h4>{{ info.cnpj }}</h4>
      </div>

      <div :class="[styles.rightContent]">
        <h3>{{ info.copyright }}</h3>
      </div>
    </div>

    <button class="to-top-btn" @click="scrollToTop">
      <img src="@/assets/arrow-up.svg" alt="Back to Top" />
    </button>
  </footer>
</template>

<script>
import styles from './TheFooter.module.scss';

export default {
  name: 'TheFooter',
  data() {
    return {
      styles,
      info: {
        cnpj: 'CNPJ: 04.487.685/0001-01',
        copyright: 'Copyright 2021 © Renee Trajar - Todos os direitos reservados.',
      },
    };
  },
  methods: {
    scrollToTop() {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    },
  },
};
</script>
