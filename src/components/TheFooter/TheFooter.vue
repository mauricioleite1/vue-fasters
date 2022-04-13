<template>
  <footer :class="[styles.container]">
    <div :class="[styles.wrapper]">
      <div :class="[styles.leftContent]">
        <img src="@/assets/footer-logo.svg" alt="Renee Trajar Logo" />
        <h4>CNPJ: 04.487.685/0001-01</h4>
      </div>

      <div :class="[styles.rightContent]">
        <h3>Copyright 2021 © Renee Trajar - Todos os direitos reservados.</h3>
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
    return { styles };
  },
  methods: {
    scrollToTop() {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    },
  },
};
</script>
