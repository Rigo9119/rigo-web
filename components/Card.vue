<template>
  <div class="card">
<!--     <picture class="card__img-wrapper">
      <img src="" alt="" class="card__img-wrapper__img">
    </picture> -->
    <h4 class="card__title headline--2">
      {{title}}
    </h4>
    <Paragraph
      class="card__paragraph"
      :paragraph="description"/>
    <Paragraph
      class="card__paragraph"
      :paragraph="role"/>
    <a class="card__link"
      :href="url"
      target="_blank">
      View
    </a>
    <h4 class="card__label">
      build with:
    </h4>
    <ul class="card__list" >
      <li v-for="item in techs"
        :key="item.id"
        class="card__list__item">
        {{item.tech}}
      </li>
    </ul>
  </div>
</template>

<script>
import Paragraph from '../components/Paragraph'

export default {
  props: {
    title: {type: String, default: ''},
    description: {type: String, default: ''},
    role: {type: String, default: ''},
    url: {type: String, default: ''},
    techs: {type: Array}
  },

  components: {
    Paragraph
  }
}
</script>

<style lang="scss" scoped>
  .card {
    align-items: flex-start;
    border: 1px solid $monza;
    display: flex;
    flex-flow: column wrap;
    justify-content: space-around;
    padding: 20px;
    height: 65vh;

    &__title {
      border-bottom: 3px solid $monza;
      color: $monza;
      padding: 10px;
    }

    &__paragraph {
      margin-top: 15px;
    }

    &__link {
      border: 1px solid $monza;
      color: $monza;
      padding: 10px;

      &:hover {
        background-color: black;
        border: 1px solid $black;
        color: $white;
      }
    }

    &__label {}

    &__list {
      &__item {
        margin-bottom: 7px;
      }
    }
  }
</style>
