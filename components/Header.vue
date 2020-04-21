<template>
  <div class="header">
    <nuxtLink to="/">
      <h1 class="header__title">
        <span class="header__title__symbol">
          &#62
        </span>
        HI I AM RIGO
      </h1>
    </nuxtLink>
    <nav class="header__nav">
      <nuxt-link class="header__nav__link" to="./about">About</nuxt-link>
      <nuxt-link class="header__nav__link" to="./skills">Skills</nuxt-link>
      <nuxt-link class="header__nav__link" to="">Portafolio</nuxt-link>
      <nuxt-link class="header__nav__link" to="">Contact</nuxt-link>
    </nav>
  </div>
</template>

<script>
  export  default {

  }
</script>

<style lang="scss">
    .header {
      align-items: flex-start;
      background: $white;
      display: flex;
      flex-flow: column nowrap;
      height: 80px;
      position: fixed;
      width: 100%;
      z-index: 1;

      @include from(desktop) {
        flex-flow: row nowrap;
        justify-content: space-between;
      }

      &__title {
        color: $monza;
        letter-spacing: 0.5px;
        padding: 15px 10px 6px 10px;
        @include font-size(22);
        width: 100%;

        @include from(desktop) {
          letter-spacing: 2px;
          @include font-size(28);
          width: 100%;
        }

        &__symbol {
          animation: pulse 0.7s infinite;
        }
      }

      &__nav {
        align-items: center;
        display: flex;
        flex-flow: row nowrap;
        justify-content: space-between;
        padding: 6px 3px ;
        width: 100%;

        @include from(desktop) {
          justify-content: flex-end;
          padding: 20px;
          width: 40%;
        }

        &__link {
          color: $monza;
          text-align: center;
          width: 25%;
          @include font-size(18);

          @include from(desktop) {
            width: 20%;
          }
        }
      }
    }
</style>
