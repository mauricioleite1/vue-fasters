<template>
  <div :class="[styles.container]">
    <img src="@/assets/whatsapp-icon.svg" alt="Um ícone para contato no Whatsapp" />
  </div>
</template>

<script>
import styles from './WhatsappIcon.module.scss';

export default {
  name: 'WhatsappIcon',
  data() { return { styles }; },
};
</script>
