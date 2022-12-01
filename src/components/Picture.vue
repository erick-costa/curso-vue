<template>
  <img :src="avatar" :alt="alt" :title="alt" />
  <Reuse />
</template>

<script>
import Reuse from "./Reuse.vue"

export default {
  name: "Picture",
  data() {
    return {
      avatar: "/img/avatar.png",
      alt: "Erick Costa",
    }
  },
  components: { Reuse },
}
</script>
