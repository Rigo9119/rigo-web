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
  </div>
</template>

<script>
  export  default {

  }
</script>

<style lang="scss">
    .header {
      background: $black;
      height: 80px;
      position: fixed;
      width: 100%;
      z-index: 1;

      &__title {
        color: $monza;
        letter-spacing: 2px;
        padding: 20px;
        @include font-size(32);
        width: 100%;

      }
    }
</style>
