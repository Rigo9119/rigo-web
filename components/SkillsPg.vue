<template>
  <div class="skills g-padding">
    <h2 class="skills__title title">
      _SKILLS AND KNOWLEDGE
    </h2>
    <p class="skills__paragraph paragraph">
      Thanks to that I have obtained skills in HTML, CSS, Javascript and some JS frameworks like React and Vue
      (this website was built with nuxt.js), also I have worked with Scrum methodologies and I like working in a team
      as I believe it helps me to learn new things.
    </p>
    <p class="skills__paragraph paragraph">
      Git is part of my workflow and is something that im trying to learn more, currently i like to use some of my
      free time to learn more Javascript and it's frameworks, graphql and Node js, i know a little bit of Ruby but to
      be honest I dont use that much as right know I want to be a Javascript developer.
    </p>
    <Button text="Go back" class="skills__button" to="/"/>
  </div>
</template>

<script>
    import Button from "./Button";

    export default {
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
        color: $oslo-gray;
      }
    }
  }
</style>
