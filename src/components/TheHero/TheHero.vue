<template>
  <div :class="[styles.container]">
    <div :class="[styles.text]">
      <h3 :class="[styles.goldenText]">Elegante é ter um</h3>
      <h3 :class="[styles.blueText]">ALFAIATE</h3>
      <h3 :class="[styles.goldenText]">para chamar de seu.</h3>
    </div>

    <div :class="[styles.callToActionTextAndButton]">
      <p>
        Compre hoje, <strong>pague em até 3x</strong><br>
        com 12% de desconto e tenha<br>
        10 meses para confeccionar!
      </p>

      <button>Faça já um orçamento</button>
    </div>

  </div>
</template>

<script>
import styles from './TheHero.module.scss';

export default {
  name: 'TheHero',
  data() {
    return {
      styles,
    };
  },
};
</script>
