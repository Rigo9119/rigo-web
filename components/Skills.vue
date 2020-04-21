<template>
  <div class="skills g-padding">
    <Title
      class="skills__title title"
      title="_SKILLS AND KNOWLEDGE"/>
    <Paragraph
      class="skills__paragraph paragraph"
      paragraph="Thanks to that I have obtained skills in HTML, CSS, Javascript and some JS frameworks like React and Vue
        (this website was built with nuxt.js), also I have worked with Scrum methodologies and I like working in a team
        as I believe it helps me learn new things."/>
    <Button text="See more" class="skills__button" to="Skills"/>
  </div>
</template>

<script>
  import Title from './Title'
  import Paragraph from "./Paragraph";
  import Button from '../components/Button'

  export default  {
    components: {
      Title,
      Paragraph,
      Button
    }
  }
</script>

<style lang="scss">
  .skills {
    align-items: flex-start;
    display: flex;
    flex-flow: column nowrap;
    justify-content: space-between;
    height: 90vh;
    width: 100vw;

    &__title {
      align-self: flex-end;
      color: $black;
    }

    &__paragraph {
      color: $black;
    }

    &__list {
      align-items: flex-start;
      display: flex;
      flex-flow: column nowrap;
      justify-content: space-evenly;
      width: 100%;

      &__item {
        color: $black;
      }
    }

    &__button {
      align-self: flex-start;
      border: 1px solid $black;
      color: $black;

      &:hover {
        background: black;
        color: $white;
      }
    }
  }
</style>
