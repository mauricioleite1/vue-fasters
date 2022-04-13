<template>
  <header :class="{ 'new-header': !showHeader }">
    <div :class="showHeader ? 'header-wrapper' : 'header-white-wrapper'">
      <div :class="[styles.logo]">
        <!-- <Logo /> -->
        <img src="@/assets/logo.svg" alt="" v-if="showHeader" />
        <img src="@/assets/min-logo.svg" alt="" v-else />
      </div>

      <div @click="showModalMenu()" @keydown="showModalMenu()">
        <img :class="[styles.hamburger]" src="@/assets/hamburger-menu.svg" alt="" />
      </div>

      <div :class="[styles.modalMenu]" v-if="showMenu">
        <div :class="[styles.modalMenuHeader]" @click="showModalMenu()" @keydown="showModalMenu()">
          <div :class="[styles.modalMenuCloseButton]">
            <img src="@/assets/close-button.svg" alt="" />
          </div>
        </div>
        <div :class="[styles.menu]">
          <a
            v-for="{ id, name, link } in navMenuOptions"
            :key="id"
            :href="link"
            @click="showModalMenu()"
            @keydown="showModalMenu()"
          >
            <h1>
              {{ name }}
            </h1>
          </a>
          <div :class="[styles.contacts]">
              <h2>Telefones</h2>
              <h4>{{ contacts.tel }}</h4>

              <h2>E-mail</h2>
              <h4>{{ contacts.email }}</h4>
            </div>
      </div>
        </div>

      <nav>
        <a v-for="{ id, name, link } in navMenuOptions" :key="id" :href="link">
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
      showMenu: false,
      contacts: {
        title: 'Contato',
        tel: '+55 (11) 3088-0757',
        email: 'renee@reneetrajar.com.br',
      },
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
    showModalMenu() {
      this.showMenu = !this.showMenu;
    },
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
