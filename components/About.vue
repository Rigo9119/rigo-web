<template>
    <div class="about g-padding">
      <Title
        class="about__title title"
        title="_ABOUT ME"/>
      <Paragraph
        class="about__paragraph paragraph"
        paragraph="I am a front end developer currently located in Bogotá Colombia, I have been working as a web developer for almost two years and a half. Currently I work at Globant as a Web UI developer and I was part of the team that was remodeling and updating the ESPN web application. "/>
      <Button text="See more" class="about__button" to="About"/>
    </div>
</template>

<script>
  import Title from "./Title"
  import Paragraph from "./Paragraph";
  import Button from './Button';

  export default  {
    components: {
      Title,
      Paragraph,
      Button
    }
  }
</script>

<style lang="scss">
  .about {
    align-items: flex-start;
    display: flex;
    flex-flow: column nowrap;
    justify-content: space-around;
    height: 90vh;
    width: 100%;
    z-index: 0;

    @include from(desktop) {
      justify-content: space-around;
    }

    &__title {
      color: $black;
    }

    &__paragraph {
      color: $black;

      &__language {
        border-bottom: 1px solid $white;
        &:hover {
          color: $monza;
          border-bottom: 1px solid $monza;
        }
      }
    }

    &__button {
      align-self: flex-end;
      border: 1px solid $black;
      color: $black;

      &:hover {
        background: $black;
        color: $white;
      }
    }
  }
</style>
