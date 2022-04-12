<template>
  <div :class="[styles.container]">
    <div :class="[styles.wrapper]">
      <div>
        <img src="@/assets/icons-1.svg" alt="" />
        <h2>Qualidade</h2>
        <p>Camisaria e Alfaiataria 100% artesanal.</p>
      </div>
      <hr>
      <div>
        <img src="@/assets/icons-2.svg" alt="" />
        <h2>Confiança</h2>
        <p>Atendimento personalizado no escritório ou residência.</p>
      </div>
      <hr>
      <div>
        <img src="@/assets/icons-3.svg" alt="" />
        <h2>Experiência</h2>
        <p>Tradição e modernidade proporcionando elegância.</p>
      </div>
    </div>
  </div>
</template>

<script>
import styles from './IconsSection.module.scss';

export default {
  name: 'IconsSection',
  data() {
    return {
      styles,
    };
  },
};
</script>
