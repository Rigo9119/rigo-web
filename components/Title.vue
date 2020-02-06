<template>
      <h2 class="title">
        {{ title }}
      </h2>
</template>

<script>
    export default {
      name: "Title",
      props: {
          title: {
            type: String,
            default: ''
          }
      }
    }
</script>

<style lang="scss">
  .title {
    color: $white;
  }
</style>
