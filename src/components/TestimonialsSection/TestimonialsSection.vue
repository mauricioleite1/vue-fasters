<template>
  <div :class="[styles.container]">
    <h1>Depoimentos</h1>
    <hr>

    <div :class="[styles.photo]" />
      <p>
        “Sou cliente do Renee há uns 12 anos.
        Nosso primeiro contato foi por intermédio de<br>meu pai,
        que já tem uma história de décadas com o querido Renee.<br>
        O excelente atendimento antes e pós venda e a alta qualidade dos materiais
        usados<br> colocam a Renee Trajar em um patamar acima dos demais do ramo.”
      </p>

    <h3>Nome</h3>
    <h4>Título da pessoa</h4>

    <div>Seleção</div>
  </div>
</template>

<script>
import styles from './TestimonialsSection.module.scss';

export default {
  name: 'TestimonialsSection',
  data() {
    return {
      styles,
    };
  },
};
</script>
