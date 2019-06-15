<template lang="pug">
  div
    section.hero.is-light.is-fullheight.is-bold
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
@import url('https://fonts.googleapis.com/css?family=M+PLUS+Rounded+1c&display=swap');
div {
  font-family: 'M PLUS Rounded 1c', sans-serif;
}

.hero-body h1 {
  font-size: 5rem;
}
</style>
