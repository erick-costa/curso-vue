<template>
  <div>
    <button
      @click="
        first('Primeiro evento', $event),
          second('Segundo evento', $event),
          third()
      "
    >
      Ativar múltiplos eventos
    </button>
    <p>{{ multiple_events }}</p>
  </div>
</template>

<script>
export default {
  name: "MultipleEvents",
  data() {
    return {
      multiple_events: "",
    }
  },
  methods: {
    first(txt, e) {
      this.multiple_events = txt
    },
    second(txt, e) {
      setTimeout(() => (this.multiple_events = txt), 500)
    },
    third() {
      setTimeout(() => (this.multiple_events = ""), 1500)
    },
  },
}
</script>

<style scoped>
div {
  margin: 100px;
}
</style>
