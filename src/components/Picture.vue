<template>
  <img :src="avatar" :alt="alt" :title="alt" />
</template>

<script>
export default {
  name: "Picture",
  data() {
    return {
      avatar: "/img/avatar.png",
      alt: "Erick Costa",
    }
  },
}
</script>
