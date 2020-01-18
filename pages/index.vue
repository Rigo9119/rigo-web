<template>
  <div>
    <div class="body">
      <About />
      <Skills />
      <Contact />
    </div>
  </div>
</template>

<script>
  import Header from '../components/Header';
  import About from '../components/About';
  import Skills from '../components/Skills';
  import Contact from '../components/Contact';

  export default {
    layout: 'default',
    components: {
      Header,
      About,
      Skills,
      Contact
    }
  }
</script>

<style lang="scss">

</style>
