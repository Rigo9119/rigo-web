<template>
    <div class="about g-padding">
      <h2 class="about__title title">
        _ABOUT
      </h2>
      <p class="about__paragraph paragraph">
        I am a front end developer currently located in Bogotá Colombia, I have been working as a web developer for
        almost two years and a half.
      </p>
      <Button text="See more" class="about__button"/>
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
  .about {
    align-items: flex-start;
    background: $river-bed;
    display: flex;
    flex-flow: column nowrap;
    justify-content: space-between;
    width: 100vw;

    &__title {
      color: $white;
    }

    &__paragraph {
      color: $white;
    }

    &__button {
      align-self: flex-end;
      border: 1px solid $white;
      color: $white;
    }
  }
</style>
