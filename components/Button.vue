<template>
  <nuxt-link class="button" :to="to">{{ text }}</nuxt-link>
</template>

<script>
  export default {
    props: {
      text: {
        type: String,
        default: ''
      },

      to: {
        type: String,
        default: ''
      }
    }
  }
</script>

<style lang="scss">
  .button {
    background: none;
    padding: 18px 28px;
    outline: none;
    text-decoration: none;
    @include font-size(20);

    &:hover {
      animation: moveTop 0.7s forwards;
    }
  }
</style>
