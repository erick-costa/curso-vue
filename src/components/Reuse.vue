<template>
  <div>
    <button @click="activate">Clique aqui!</button>
    <span v-show="activated">Ativado!</span>
  </div>
</template>

<script>
export default {
  name: "Reuse",
  data() {
    return {
      activated: false,
    }
  },
  methods: {
    activate() {
      this.activated = !this.activated
    },
  },
}
</script>
