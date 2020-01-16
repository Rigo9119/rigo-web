<template>
  <div class="skills g-padding">
    <h2 class="skills__title title">
      _SKILLS
    </h2>
    <p class="skills__paragraph paragraph">
      Thanks to that I have obtained skills in HTML, CSS, SCSS, Javascript and some JS frameworks like React and Vue
      (this website is built with nuxt.js)
    </p>
    <Button text="See more" class="skills__button" />
  </div>
</template>

<script>
  import Button from '../components/Button'

  export default  {
    components: {
      Button
    }
  }
</script>

<style lang="scss">
  .skills {
    align-items: flex-start;
    background: $oslo-gray;
    display: flex;
    flex-flow: column nowrap;
    justify-content: space-between;
    width: 100vw;

    &__title {
      align-self: flex-end;
      color: $black;
    }

    &__paragraph {
      color: $black;
    }

    &__button {
      align-self: flex-start;
      border: 1px solid $black;
      color: $black;
    }
  }
</style>
