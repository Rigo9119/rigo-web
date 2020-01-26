<template>
    <div class="contact g-padding">
      <h2 class="contact__title title">_CONTACT</h2>
      <P class="contact__paragraph paragraph">
        As I mentioned before I am currently located in Bogotá Colombia, but you can contact me by the following
      </P>
      <div class="contact__menu">
        <a href="" class="contact__menu__item">LinkedIn</a>
        <a href="" class="contact__menu__item">Glassdor</a>
      </div>
    </div>
</template>

<scrip>
</scrip>

<style lang="scss">
  .contact {
    align-items: flex-start;
    background: $monza;
    display: flex;
    flex-flow: column nowrap;
    height: 90vh;
    justify-content: space-between;
    width: 100vw;

    &__title {
      color: $oslo-gray;
    }

    &__paragraph {
      color: $oslo-gray;
    }

    &__menu {
      align-items: center;
      display: flex;
      flex-flow: row nowrap;
      justify-content: space-evenly;
      margin: 30px auto;
      width: 100%;

      &__item {
        align-self: center;
        color: $oslo-gray;
        margin-bottom: 60px;
        padding: 18px 28px;
        @include font-size(20);

        @include from(desktop) {
          margin-bottom: 0;
        }

        &:hover {
          background: $oslo-gray;
          color: $monza;
        }
      }
    }
  }
</style>
