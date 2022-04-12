<template>
  <header>
    <div>
      <h2>Logo</h2>
    </div>

    <nav>
      <a href="">EMPRESA</a>
      <a href="">CAMISARIA</a>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'TheHeader',
  data() {
    return {
      socialLinks: [
        {
          name: 'logo-instagram',
          link: 'https://www.instagram.com/mauricioleite1',
        },
        {
          name: 'logo-linkedin',
          link: 'https://www.linkedin.com/in/mauricioleite',
        },
        {
          name: 'logo-github',
          link: 'https://www.github.com/mauricioleite1',
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./TheHeader.scss";
</style>
