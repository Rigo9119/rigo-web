<template>
  <div class="header">
    <nuxtLink to="/" :class="{ hide: toggle }">
      <h1 class="header__title">
        <span class="header__title__symbol">
          &#62;
        </span>
        HI I AM RIGO
      </h1>
    </nuxtLink>
    <Nav :class="{ show: toggle }"/>
    <button class="header__button" :class="{ hide: toggle }" @click="toggle=true">
      &#60;
    </button>
    <button class="header__button hide" :class="{ show: toggle }" @click="toggle=false">
      &#62;
    </button>
  </div>
</template>

<script>
import Nav from './Nav'

export  default {
  components: {
    Nav
  },

  data () {
    return {
      toggle: false
    }
  },

  methods: {
    toggleMenu: (event) => {
      this.toggle = !this.toggle
    }
  }
}
</script>

<style lang="scss">
  .header {
    align-items: center;
    background: $white;
    display: flex;
    flex-flow: row nowrap;
    height: 80px;
    justify-content: space-between;
    position: fixed;
    width: 100%;
    z-index: 1;

    @include from(desktop) {

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


    &__button {
      align-self: center;
      background: none;
      border: none;
      color: $monza;
      margin-right: 10px;
      outline: none;
      text-align: center;
      @include font-size(32);

      @include from(desktop) {
        padding: 15px;
        display: none;
      }
    }

    .hide {
      display: none;
    }

    .show {
      display: flex;
    }
  }

</style>
