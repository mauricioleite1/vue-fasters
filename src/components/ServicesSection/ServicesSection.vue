<template>
  <div :class="[styles.container]">
    <div :class="[styles.top]">

      <div :class="[styles.image]">
        <div :class="[styles.imgBorder]" />
        <div :class="[styles.imgCamisaria]" />
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

    <div :class="[styles.bottom]">

      <div :class="[styles.imageInfo]">
        <div id="camisaria" :class="[styles.camisaria]">
          <div :class="[styles.title]">
            <h1>Alfaiataria</h1>
            <h5>- Totalmente feito à mão sob medida</h5>
          </div>

          <div :class="[styles.lists]">
            <ul>
              <li>Fio Super 120 e 130</li>
              <li>Lã fria Australiana</li>
              <li>Botões Importados</li>
            </ul>
            <ul>
              <li>Ternos e Calças</li>
              <li>Paletós e Smokings</li>
              <li>Sociais e Esportivos</li>
            </ul>
          </div>
        </div>
          <button>Quero um orçamento</button>
      </div>
      <div :class="[styles.image]">
        <div :class="[styles.imgBorder]" />
        <div :class="[styles.imgAlfaiataria]" />
        <!-- <img src="@/assets/services-2.jpg" alt="" /> -->
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
