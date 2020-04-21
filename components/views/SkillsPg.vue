<template>
  <div class="skills g-padding">
    <h2 class="skills__title title">
      _SKILLS
    </h2>

    <!-- basic skills -->
    <ul class="skills__list">
      <h4 class="skill__list__title">Basics:</h4>
      <li v-for="skill in basics" v-bind:key="skill.name" class="skills__list__item">{{skill.name}}</li>
    </ul>

    <!-- HTML skills -->
    <ul class="skills__list">
      <h4 class="skill__list__title">HTML:</h4>
      <li v-for="skill in html" v-bind:key="skill.name" class="skills__list__item">{{skill.name}}</li>
    </ul>

    <!-- CSS skills -->
    <ul class="skills__list">
      <h4 class="skill__list__title">CSS:</h4>
      <li v-for="skill in css" v-bind:key="skill.name" class="skills__list__item">{{skill.name}}</li>
    </ul>

    <!-- javascript skills -->
    <ul class="skills__list">
      <h4 class="skill__list__title">Javascript:</h4>
      <li v-for="skill in js" v-bind:key="skill.name" class="skills__list__item">{{skill.name}}</li>
    </ul>

    <!-- frameworks skills -->
    <ul class="skills__list">
      <h4 class="skill__list__title">Frameworks:</h4>
      <li v-for="skill in frameworks" v-bind:key="skill.name" class="skills__list__item">{{skill.name}}</li>
    </ul>

    <!-- other skills -->
    <ul class="skills__list">
      <h4 class="skill__list__title">Others:</h4>
      <li v-for="skill in others" v-bind:key="skill.name" class="skills__list__item">{{skill.name}}</li>
    </ul>
    <Button text="Go back" class="skills__button" to="/"/>
  </div>
</template>

<script>
    import Button from "../Button";

    export default {
      components: {
        Button
      },

      data() {
        return {
          basics: [{name: 'HTML'}, {name: 'CSS'}, {name: 'Javascript'}, {name: 'Git / Github'}],
          html: [{name: 'Accesibility'}, {name: 'Forms'}, {name: 'Semanthic HTML'}],
          css: [{name: 'Flexbox'}, {name: 'CSS Grid'}, {name: 'Mobile first'}, {name: 'Responsive Desgin'}, {name: 'SCSS / SASS'}, {name: 'CSS Animations'}, {name: 'Bootstrap'}],
          js: [{name: 'ES6'}, {name: 'OOP'}, {name: 'Functional programming'}],
          frameworks: [{name: 'React'}, {name: 'Vue Js'}, {name: 'Next Js'}, {name: 'Nuxt Js'}, {name: 'Gatsby Js'}],
          others: [{name: 'Scrum methodology'}, {name: 'Storybook'}, {name: 'Emotion Js'}, {name: 'Node Js'}, {name: 'Graphql'}]
        }
      }
    }

</script>

<style lang="scss">
  .skills {
    align-items: flex-start;
    display: flex;
    flex-flow: column nowrap;
    justify-content: space-between;
    height: 120vh;
    width: 100vw;

    &__title {
      align-self: flex-start;
      color: $black;
      width: 100%;
    }

    &__list {
      align-items: center;
      display: flex;
      flex-flow: column nowrap;
      justify-content: center;
      width: 100%;

      &--left {
        justify-self: flex-end;
      }

      &__title {
        color: $black;
        margin-bottom: 10px;
      }

      &__item {
        color: $black;
        margin-bottom: 5px;
        letter-spacing: 1px;
      }
    }

    &__button {
      align-self: flex-start;
      border: 1px solid $black;
      color: $black;
      margin-top: 40px;

      &:hover {
        background: black;
        color: $oslo-gray;
      }
    }
  }
</style>
