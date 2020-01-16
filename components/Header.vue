<template>
  <div class="name">
    <h1 class="name__title">
      <span class="name__title__symbol">
        &#62
      </span>
      HI I AM RIGO
    </h1>
  </div>
</template>

<script>

</script>

<style lang="scss">
    .name {
      background: $black;
      width: 100%;

      &__title {
        color: $monza;
        letter-spacing: 2px;
        padding: 30px;
        @include font-size(32);
        width: 100%;

      }
    }
</style>
