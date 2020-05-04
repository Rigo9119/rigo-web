<template>
  <div class="skillspg g-padding">
    <h2 class="skillspg__title title">
      _SKILLS
    </h2>
    <Paragraph
      class="skillspg__paragraph"
      paragraph="Most of my dev Skills are related to Front End Development but im doing my best and try to learn new things."/>
    <Paragraph
      class="skillspg__paragraph"
      paragraph="Here is a list of my skills:" />
    <div class="skillspg__wrapper">
      <!-- basic skills -->
      <ul class="skillspg__wrapper__list">
        <h4 class="skillspg__wrapper__list__title"></h4>
        <li v-for="skill in skills" v-bind:key="skill.name" class="skillspg__wrapper__list__item">{{skill.name}}</li>
      </ul>
      <!-- other skills -->
      <ul class="skillspg__wrapper__list">
        <h4 class="skillspg__wrapper__list__title">Others:</h4>
        <li v-for="skill in others" v-bind:key="skill.name" class="skillspg__wrapper__list__item">{{skill.name}}</li>
      </ul>
    </div>
    <Button text="Go back" class="skillspg__button" to="/"/>
  </div>
</template>

<script>
    import Button from "../Button";
    import Paragraph from "../Paragraph";
    export default {
      components: {
        Button,
        Paragraph
      },

      data() {
        return {
          skills: [
            {name: 'HTML'},
            {name: 'CSS'},
            {name: 'SCSS / SASS'},
            {name: 'Javascript'},
            {name: 'Git / Github'},
            {name: 'React'},
            {name: 'Gatsby JS'},
            {name: 'Next JS'},
            {name: 'Vue JS'},
            {name: 'Nuxt JS'}
          ],
          others : [
            {name: 'Node Js (basic)'},
            {name: 'Graphql (basic)'},
            {name: 'Storybook'},
            {name: 'Styled Components / Emotion Js'},
            //{name: 'Ruby (basic)'}
          ]
        }
      }
    }

</script>

<style lang="scss">
  .skillspg {
    align-items: flex-start;
    display: flex;
    flex-flow: column nowrap;
    justify-content: space-between;
    height: auto;
    width: 100vw;

    &__title {
      align-self: flex-start;
      color: $black;
      width: 100%;
    }

    &__paragraph {
      padding-top: 10px;
    }

    &__wrapper {
      align-items: center;
      display: flex;
      flex-flow: column nowrap;
      justify-content: center;
      width: 100%;

      @include from(desktop) {
        flex-flow: row nowrap;
      }

      &__list {
        align-items: center;
        display: flex;
        flex-flow: column nowrap;
        justify-content: center;
        padding-top: 15px;
        width: 100%;

        &--left {
          @include from(desktop) {
            justify-self: flex-start;
          }
        }

        &--right {
          @include from(desktop) {
            justify-self: flex-end;
          }
        }

        &--center {
          @include from(desktop) {
            justify-self: center;
          }
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
