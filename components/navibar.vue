<template lang="pug">
  nav.navbar
    .navbar-brand
      a(role="button" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample" @click="toggle").navbar-burger.burger
        span.has-text-danger
        span.has-text-danger
        span.has-text-danger

    .navbar-menu#navbarBasicExample
      .navbar-end
        a.navbar-item(href="/motorisierte-schleife") Home
        a.navbar-item(href="/motorisierte-schleife/about") About
        .navbar-item.has-dropdown.is-hoverable
          a.navbar-link Works
          .navbar-dropdown
            a.navbar-item(href="/motorisierte-schleife/works/discography") Discography
            a.navbar-item(href="/motorisierte-schleife/works/software") Software

        span.navbar-item
          a.button.is-black.is-inverted(href="https://github.com/ChefyHase")
            span.icon
              i.fab.fa-github
            span GitHub
        span.navbar-item
          a.button.is-black.is-inverted(href="https://www.nicovideo.jp/user/89543587")
            span.icon
              i.fas.fa-play
            span NicoNico
        span.navbar-item
          a.button.is-link.is-inverted(href="https://twitter.com/haru__futaba")
            span.icon
              i.fab.fa-twitter
            span Twitter
</template>

<script>
export default {
  methods: {
    toggle() {
      const $navbarBurgers = Array.prototype.slice.call(
        document.querySelectorAll('.navbar-burger'),
        0
      )

      // Check if there are any navbar burgers
      if ($navbarBurgers.length > 0) {
        // Add a click event on each of them
        $navbarBurgers.forEach(el => {
          // Get the target from the "data-target" attribute
          const target = el.dataset.target
          const $target = document.getElementById(target)

          // Toggle the "is-active" class on both the "navbar-burger" and the "navbar-menu"
          el.classList.toggle('is-active')
          $target.classList.toggle('is-active')
        })
      }
    }
  }
}
</script>
