<template>
  <div class="about g-padding">
    <h2 class="about__title title">
      _ABOUT ME
    </h2>
    <p class="about__paragraph paragraph">
      You would think I have a background of IT or something related but actually I have a bachelor of recording
      arts, and im learning this web development things all by my self. I like technology and how it can help people to
      develop new stuff
    </p>
    <Button text="Go back" class="about__button" to="/"/>
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
  .about {
    align-items: flex-start;
    background: $black;
    display: flex;
    flex-flow: column nowrap;
    justify-content: space-between;
    height: 100vh;
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
