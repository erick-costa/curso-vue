<template>
  <h2>Essa é a descrição da pessoa: {{ name }}</h2>
  <Info />
</template>

<script>
import Info from "./Info.vue"

export default {
  name: "Person",
  components: {
    Info,
  },
  data() {
    return {
      name: "Erick",
    }
  },
}
</script>
