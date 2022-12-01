<template>
  <img :src="avatar" :alt="alt" :title="alt" />
  <Changeimage @change-image="changeImage" />
</template>

<script>
import Changeimage from "./Changeimage.vue"

export default {
  name: "Picture",
  data() {
    return {
      avatar: "/img/avatar.png",
      alt: "Erick Costa",
    }
  },
  components: { Changeimage },
  methods: {
    changeImage() {
      this.avatar = "/img/avatar2.png"
    },
  },
}
</script>
