<template>
  <p v-if="is_working">Estou trabalhando no momento.</p>
  <p v-else>Estou em busca de novas oportunidades</p>
  <p>Utilizo as seguintes tecnologias:</p>
  <ul>
    <li>JavaScript</li>
    <li>Python</li>
    <li>React.js</li>
    <li>Vue.js</li>
  </ul>
  <p v-show="show_email">Mande uma mensagem para: {{ email }}</p>
  <p>
    Para acessar meu portfólio, basta clicar
    <a v-bind:href="my_link" target="_blank"> aqui</a>
  </p>
  <Picture />
</template>

<script>
import Picture from "./Picture.vue"
export default {
  name: "Info",
  components: {
    Picture,
  },
  data() {
    return {
      is_working: true,
      show_email: true,
      email: "erick@email.com",
      my_link: "https://github.com/erick-costa",
    }
  },
}
</script>
