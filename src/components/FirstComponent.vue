<template>
  <h1>Olá Vue!</h1>
  <p>Meu nome é: {{ name }}</p>
  <MultipleEvents />
</template>

<script>
import MultipleEvents from "./MultipleEvents.vue"

export default {
  name: "FirstComponent",
  components: {
    MultipleEvents,
  },
  data() {
    return {
      name: "Erick",
    }
  },
}
</script>
