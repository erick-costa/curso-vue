<template>
  <h2>Essa é a descrição da pessoa: {{ name }}</h2>
  <Info :email="email" :is_working="false" />
  <Form />
</template>

<script>
import Info from "./Info.vue"
import Form from "./Form.vue"

export default {
  name: "Person",
  components: {
    Info,
    Form,
  },
  data() {
    return {
      name: "Erick",
      email: "erick@email.com",
    }
  },
}
</script>
