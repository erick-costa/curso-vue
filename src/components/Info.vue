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
</template>

<script>
export default {
  name: "Info",
  data() {
    return {
      is_working: true,
      show_email: true,
      email: "erick@email.com",
    }
  },
}
</script>
