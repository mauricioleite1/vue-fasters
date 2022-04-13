<template>
  <div id="contato" :class="[styles.container]">
    <div :class="[styles.titulo]">
      <h1>{{ contacts.title }}</h1><hr />
    </div>

    <div :class="[styles.content]">
      <div :class="[styles.leftWrapper]">
        <div :class="[styles.leftContent]">

          <div :class="[styles.contacts]">
            <h2>Telefones</h2>
            <h4>{{ contacts.tel }}</h4>

            <h2>E-mail</h2>
            <h4>{{ contacts.email }}</h4>
          </div>

          <div :class="[styles.callToActionButton]">
            <h2>Atendimento Personalizado</h2>
            <button class="contact-btn">Clique aqui!</button>
          </div>

        </div>
      </div>

      <div :class="[styles.rightWrapper]">
        <form>
          <label v-for="{ id, title, placeholder } in inputs" :key="id" :for="title">
            <input type="text" :v-model="title" :placeholder="placeholder" />
          </label>

          <button>{{ button }}</button>
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
    return {
      inputs: [
        { id: 1, title: 'name', placeholder: 'Nome' },
        { id: 2, title: 'email', placeholder: 'E-mail' },
        { id: 3, title: 'message', placeholder: 'Mensagem' },
      ],
      contacts: {
        title: 'Contato',
        tel: '+55 (11) 3088-0757',
        email: 'renee@reneetrajar.com.br',
      },
      button: 'Enviar Mensagem',
      styles,
      name: '',
      email: '',
      message: '',
    };
  },
};
</script>
