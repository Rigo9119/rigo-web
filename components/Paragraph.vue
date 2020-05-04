<template>
    <p class="paragraph">
      {{ paragraph }}
    </p>
</template>

<script>
    export default {
      name: "Paragraph.vue",
      props: {
        paragraph: {
          type: String,
          default: ' ',
        }
      }
    }
</script>

<style lang="scss" scoped>

</style>
