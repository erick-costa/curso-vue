<template>
  <p v-if="is_working">Estou trabalhando no momento.</p>
  <p v-else>Estou em busca de novas oportunidades</p>
  <p>Utilizo as seguintes tecnologias para back-end:</p>
  <ul>
    <li v-for="item in backend">{{ item }}</li>
  </ul>
  <p>Utilizo as seguintes tecnologias para front-end:</p>
  <ul>
    <li v-for="item in frontend">{{ item.technology }}</li>
  </ul>
  <div>
    <button @click="showEmail">{{ buttonText }}</button>
  </div>
  <p v-show="show_email">Mande uma mensagem para: {{ email }}</p>
  <p class="teste">
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
  props: {
    email: String,
    is_working: Boolean,
  },
  data() {
    return {
      show_email: false,
      my_link: "https://github.com/erick-costa",
      buttonText: "Mostrar Email",
      backend: ["JavaScript", "Python"],
      frontend: [
        { id: 1, technology: "HTML" },
        { id: 2, technology: "CSS" },
        { id: 3, technology: "React" },
        { id: 4, technology: "Vue" },
      ],
    }
  },
  methods: {
    showEmail() {
      this.show_email = !this.show_email
      if (!this.show_email) {
        this.buttonText = "Mostrar Email"
      } else {
        this.buttonText = "Esconder Email"
      }
    },
  },
}
</script>
