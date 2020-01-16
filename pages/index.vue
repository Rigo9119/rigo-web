<template>
  <div>
    <Header />
    <About />
    <Skills />
    <Contact />
  </div>
</template>

<script>
  import Header from '../components/Header';
  import About from '../components/About';
  import Skills from '../components/Skills';
  import Contact from '../components/Contact';

  export default {
    components: {
      Header,
      About,
      Skills,
      Contact
    }
  }
</script>

<style>

</style>
