<template>
    <div class="about g-padding">
      <Title
        class="about__title title"
        title="_ABOUT ME"/>
      <Paragraph
        class="about__paragraph paragraph"
        paragraph="
          I am a front end developer currently located in Bogotá Colombia, I have been working as a web developer for
          almost two years and a half. Currently I work at Globant as a Web UI dev where I am part of the team that is in
          charge of remodeling the ESPN website.
        "/>
      <p class="about__paragraph paragraph">
        I speak  <span class="about__paragraph__language">English</span >, a little of
        <span class="about__paragraph__language">Korean</span> as my wife
        is from South Korea so I learn just a bit of it, also I speak <span class="about__paragraph__language">
        Spanish</span> because is my mother tongue.
      </p>
    </div>
</template>

<script>
  import Title from "./Title"
  import Paragraph from "./Paragraph";

  export default  {
    components: {
      Title,
      Paragraph
    }
  }
</script>

<style lang="scss">
  .about {
    align-items: flex-start;
    background: $black;
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
      color: $white;
    }

    &__paragraph {
      color: $white;

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
      border: 1px solid $white;
      color: $white;

      &:hover {
        background: $white;
        color: $black;
      }
    }
  }
</style>
