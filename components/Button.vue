<template>
  <button class="button">{{ text }}</button>
</template>

<script>
  export default {
    props: {
      text: {
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
  }
</style>
