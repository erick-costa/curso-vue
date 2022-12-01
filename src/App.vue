<template>
  <Header />
  <FirstComponent />
  <LifeCycle />
  <Person />
</template>

<script>
import FirstComponent from "./components/FirstComponent.vue"
import LifeCycle from "./components/LifeCycle.vue"
import Person from "./components/Person.vue"
import Header from "./components/Header.vue"

export default {
  name: "App",
  components: {
    FirstComponent,
    LifeCycle,
    Person,
    Header,
  },
}
</script>

<style>
body {
  background-color: #333;
  color: #fff;
}

a {
  color: red;
}

.teste {
  background-color: black;
}
</style>
