<template lang="pug">
  div
    section.hero.is-fullheight.is-bold.has-bg-img
      .hero-head
        Navibar
      .hero-body
        .container
          h1.title Motorisierte Schleife
          h2.subtitle Touhou Music & Coding Circle
</template>

<script>
import Navibar from '~/components/navibar.vue'

export default {
  components: {
    Navibar
  }
}
</script>

<style>
div {
  font-family: 'M PLUS Rounded 1c', sans-serif;
}

.has-bg-img {
  background: url('~assets/indexBackground.jpg');
  background-size: cover;
  position: relative;
}

.hero-body h1 {
  font-size: 5rem;
  text-shadow: 2px 2px 2px gray;
}
</style>
