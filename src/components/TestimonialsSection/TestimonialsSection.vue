<template>
  <div id="depoimentos" :class="[styles.container]">
    <div :class="[styles.titulo]">
      <h1>Depoimentos</h1>
      <hr />
    </div>

    <div :class="[styles.photo]" />
    <p>
      “Sou cliente do Renee há uns 12 anos. Nosso primeiro contato foi por intermédio de<br />meu
      pai, que já tem uma história de décadas com o querido Renee.<br />
      O excelente atendimento antes e pós venda e a alta qualidade dos materiais usados<br />
      colocam a Renee Trajar em um patamar acima dos demais do ramo.”
    </p>

    <div :class="[styles.nome]">
      <h3>William H. M. Garey</h3>
      <h4>Advogado | Nelson Garey Avogados Associados</h4>
    </div>

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
