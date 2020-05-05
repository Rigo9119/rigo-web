<template>
  <div id="index" class="body">
    <About id="about"/>
    <Skills id="skills"/>
    <Contact id="contact"/>
  </div>
</template>

<script>
  import About from '../components/About';
  import Skills from '../components/Skills';
  import Contact from '../components/Contact';

  export default {
    layout: 'default',
    components: {
      About,
      Skills,
      Contact
    },
/*
    data: {
      scrollPosition: 0,
      active: null,
      lastActive: null,
      lastScrolltop: window.pageYOffset || document.documentElement.scrollTop,
      scrollStarted: false,
      down: true
    },

    mounted() {
      this.active = 1
      this.lastActive = 1
      window.addEventListener('scroll', this.handleScroll)
    },

    methods: {
      handleScroll(element) {
        let me = this,
            options = {
              container: 'body',
              easing: 'ease-in',
              offset: 0,
              cancelable: false,
              onStart: function () {
                document.body.style.overflow = 'hidden'
              },
              onDone: _.debounce(function(element) {
                if (me.down) me.active++
                else me.active--
                me.scrollStarted = false
                document.body.style.overflow = 'auto'
              }, 100),
              x: false,
              y: true
            },
            st = window.scrollY;
        if (st > this.lastScrollTop) {
            this.down = true
          } else {
            this.down = false
          }
          this.lastScrollTop = st
      if (!this.scrollStarted) {
        this.scrollStarted = true
        if (this.down) {
          this.down = true
          if (this.active === 1) {
            VueScrollTo.scrollTo('#skills', 500, options)
          } else if (this.active === 2) {
            VueScrollTo.scrollTo('#contact', 500, options)
          }
        } else {
          if (this.active === 2) {
            VueScrollTo.scrollTo('#about', 500, options)
          } else if (this.active === 3) {
            VueScrollTo.scrollTo('#skills', 500, options)
          } else if (this.active === 4) {
            VueScrollTo.scrollTo('#contact', 500, options)
          }
        }
      }
      }
    }, */
  }
</script>

<style lang="scss">

</style>
