<template>
  <div :class="[styles.container]">
    <div :class="[styles.wrapper]">
      <div :class="[styles.callToActionTextAndButton]">
        <h1>Condição Imperdível</h1>
        <h2>Compre hoje e garanta:</h2>
        <p>- 12% de desconto e pagamento em até <strong>3x sem juros;</strong></p>
        <p>- Até <strong>10 meses</strong> para confeccionar sua roupa. Não se preocupe se<br>
        suas medidas aumentaram ou diminuíram, estará sempre elegante;</p>
        <p>- Condição muito especial por <strong>tempo limitado</strong></p>
        <p>- Poder presentear alguém com uma roupa de alta costura, <strong>exclusiva</strong>.</p>
        <button>Garanta essa condição especial!</button>
      </div>

      <img src="@/assets/specialinfo-1.jpg" alt="" />
    </div>
  </div>
</template>

<script>
import styles from './SpecialSection.module.scss';

export default {
  name: 'IconsSection',
  data() {
    return {
      styles,
    };
  },
};
</script>
