<template>
  <div class="body">
    <About />
    <Skills />
    <Contact />
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
    }
  }
</script>

<style lang="scss">

</style>
