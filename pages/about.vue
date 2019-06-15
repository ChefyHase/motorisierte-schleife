<template lang="pug">
  div
    section.hero.is-dark.is-fullheight.is-bold
      .hero-head
        Navibar
      .hero-body
        .container
          img(src="https://pbs.twimg.com/profile_images/1139724315799117824/PSpf1EY-_400x400.png").is-center
          h1.has-text-centered.name 双羽晴
          h2.has-text-centered.aka aka. TwinFeathers
          p.has-text-centered.desp 東方アレンジ作ったりプログラミングしたりDJしたり
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

h1.name {
  font-size: 5rem;
  margin: 0;
}
h3.name {
  font-size: 2rem;
}

h2.aka {
  font-size: 3rem;
}

p.desp {
  margin: 2rem;
  font-size: 1rem;
}

.is-center {
  display: flex;
  align-items: center;
  margin: 0 auto;
}

img {
  border-radius: 50%;
  width: 15%;
  height: 15%;
}
</style>
