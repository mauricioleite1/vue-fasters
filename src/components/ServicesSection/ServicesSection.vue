<template>
  <div :class="[styles.container]">
    <div :class="[styles.top]">

      <div :class="[styles.image]">
        <div :class="[styles.imgBorder]" />
        <img src="@/assets/services-1.jpg" alt="" />
      </div>
      <div :class="[styles.imageInfo]">
        <div id="camisaria" :class="[styles.camisaria]">
          <div :class="[styles.title]">
            <h1>Camisaria</h1>
            <h5>- Confeccionadas Artesanalmente</h5>
          </div>

          <div :class="[styles.lists]">
            <ul>
              <li>100% Algodão</li>
              <li>Monograma</li>
              <li>Slim</li>
            </ul>
            <ul>
              <li>Nacionais e Importados</li>
              <li>Tradicionais e Esportivas</li>
              <li>Casamentos</li>
            </ul>
          </div>
        </div>
          <button>Quero um orçamento</button>
      </div>
    </div>
  </div>
</template>

<script>
import styles from './ServicesSection.module.scss';

export default {
  name: 'ServicesSection',
  data() {
    return {
      styles,
    };
  },
};
</script>
