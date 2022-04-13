<template>
  <header :class="{ 'new-header': !showHeader }">
    <div :class="showHeader ? 'header-wrapper' : 'header-white-wrapper'">
      <div :class="[styles.logo]">
        <!-- <Logo /> -->
        <img src="@/assets/logo.svg" alt="" v-if="showHeader" />
        <img src="@/assets/min-logo.svg" alt="" v-else />
      </div>

      <nav>
        <a
          v-for="{ id, name, link } in navMenuOptions"
          :key="id"
          :href="link">
          <h4>
            {{ name }}
          </h4>
        </a>
      </nav>
    </div>
  </header>
</template>

<script>
// import Logo from '@/assets/logo.svg';
import styles from './TheHeader.module.scss';

export default {
  name: 'TheHeader',
  data() {
    return {
      styles,
      showHeader: true,
      navMenuOptions: [
        { id: 1, name: 'EMPRESA', link: '#empresa' },
        { id: 2, name: 'CAMISARIA', link: '#camisaria' },
        { id: 3, name: 'ALFAIATARIA', link: '#alfaiataria' },
        { id: 4, name: 'DEPOIMENTOS', link: '#depoimentos' },
        { id: 5, name: 'CONTATO', link: '#contato' },
      ],
    };
  },
  created() {
    window.addEventListener('scroll', this.handleScroll);
  },
  unmounted() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      if (window.pageYOffset < 100) {
        this.showHeader = true;
      } else {
        this.showHeader = false;
      }
    },
  },
};
</script>
