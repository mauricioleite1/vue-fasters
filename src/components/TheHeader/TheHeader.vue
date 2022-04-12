<template>
  <header>
    <div :class="[styles.wrapper]">
      <div :class="[styles.logo]">
        <h2>Logo</h2>
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
import styles from './TheHeader.module.scss';

export default {
  name: 'TheHeader',
  data() {
    return {
      styles,
      navMenuOptions: [
        { id: 1, name: 'EMPRESA', link: '#empresa' },
        { id: 2, name: 'CAMISARIA', link: '#camisaria' },
        { id: 3, name: 'ALFAIATARIA', link: '#alfaiataria' },
        { id: 4, name: 'DEPOIMENTOS', link: '#depoimentos' },
        { id: 5, name: 'CONTATO', link: '#contato' },
      ],
    };
  },
};
</script>
