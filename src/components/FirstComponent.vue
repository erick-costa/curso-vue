<template>
  <h1>Olá Vue!</h1>
  <p>Meu nome é: {{ name }}</p>
</template>

<script>
export default {
  name: "FirstComponent",
  data() {
    return {
      name: "Erick",
    }
  },
}
</script>
