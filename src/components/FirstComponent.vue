<template>
  <Reuse />
  <h1>Olá Vue!</h1>
  <Reuse />
  <p>Meu nome é: {{ name }}</p>
  <MultipleEvents />
  <Reuse />
  <Reuse />
  <Reuse />
  <Reuse />
  <Reuse />
  <Reuse />
</template>

<script>
import MultipleEvents from "./MultipleEvents.vue"
import Reuse from "./Reuse.vue"

export default {
  name: "FirstComponent",
  components: {
    MultipleEvents,
    Reuse,
  },
  data() {
    return {
      name: "Erick",
    }
  },
}
</script>
