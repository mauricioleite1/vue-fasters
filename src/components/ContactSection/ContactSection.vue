<template>
  <div :class="[styles.container]">
    <div :class="[styles.titulo]">
        <h1>Contato</h1>
        <hr />
    </div>

    <div :class="[styles.content]">
      <div :class="[styles.leftWrapper]">
        <div :class="[styles.leftContent]">
          <div :class="[styles.contacts]">
            <h2>Telefones</h2>
            <h4>+55 (11) 3088-0757</h4>

            <h2>E-mail</h2>
            <h4>renee@reneetrajar.com.br</h4>
          </div>
          <div :class="[styles.callToActionButton]">
            <h2>Atendimento Personalizado</h2>
            <button class="contact-btn">Clique aqui!</button>
          </div>
        </div>
      </div>

      <div :class="[styles.rightWrapper]">
        <form>
          <label for="name">
            <input type="text" v-model="name" placeholder="Nome" />
          </label>
          <label for="email">
            <input type="text" v-model="email" placeholder="E-mail" />
          </label>
          <label for="message">
            <input type="text" v-model="message" placeholder="Mensagem" />
          </label>

          <button>Enviar Mensagem</button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
import styles from './ContactSection.module.scss';

export default {
  name: 'ContactSection',
  data() {
    return { styles };
  },
};
</script>
