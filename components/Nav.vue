<template>
  <nav class="nav">
    <nuxt-link class="nav__link" to="./about">About</nuxt-link>
    <nuxt-link class="nav__link" to="./skills">Skills</nuxt-link>
    <nuxt-link class="nav__link" to="./portafolio">Portafolio</nuxt-link>
    <!--<nuxt-link class="nav__link" to="">Contact</nuxt-link>-->
  </nav>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  .nav {
  align-items: center;
  display: none;
  flex-flow: row nowrap;
  justify-content: space-between;
  padding: 6px 10px ;
  width: 75%;

  @include from(desktop) {
    display: flex;
    justify-content: flex-end;
    padding: 20px;
    width: 40%;
  }

  &__link {
    color: $monza;
    text-align: center;
    width: 25%;
    @include font-size(22);

    @include from(desktop) {
      width: 20%;
    }
  }
}
</style>
