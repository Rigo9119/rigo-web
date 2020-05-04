<template>
  <div class="portafolio g-padding">
    <Card
      class="portafolio__card"
      title="LegalFast"
      description="Legal Fast is a web application that helps customers find a lawyer or lawfirm in colombia it is in the final stages of development"
      role="In this project I am part o the Front End dev team that help build and develop it"
      url="https://legal-fastqa.herokuapp.com/"
      :techs="legalfast"/>
    <Card
      class="portafolio__card"
      title="ESPN"
      description="It is a web plattaform for sports, in the re customers can check information about different, sports, teams, leagues and players"
      role="In this project I was part of the Web UI (Front End) team that help to maintain and update it with new technologies"
      url="https://www.espn.com.co/futbol-americano/colegial/rankings"
      :techs="espn"/>
    <Card
      class="portafolio__card"
      title="JyC Supply"
      description="It is a SPA for a logisitics company from Colombia"
      role="I helped in the initial stages, it uses the JAMStack approach"
      url="http://jycsupply.com/"
      :techs="jyc"/>
  </div>
</template>

<script>
import Card from '../Card'
export default {
  components: {
    Card
  },

  data() {
    return {
      legalfast: [
        {tech: 'Nuxt Js'},
        {tech: 'SCSS'},
        {tech: 'HTML'},
        {tech: 'Javascript'},
        {tech: 'git / gihub'}
      ],
      espn:[
        {tech: 'React'},
        {tech: 'Javascript'},
        {tech: 'CSS'},
        {tech: 'Karma(TDD/BDD)'},
        {tech: 'git / gihub'},
      ],
      jyc: [
        {tech: 'Gatsby Js'},
        {tech: 'Emotion Js'},
        {tech: 'Dato CMS'},
        {tech: 'Netlify'},
        {tech: 'git / gihub'}
      ]
    }
  }
}
</script>

<style lang="scss">
  .portafolio {
    align-items: center;
    display: flex;
    flex-flow: column wrap;
    justify-content: space-between;
    width: 100%;

    @include from(desktop) {
      flex-flow: row wrap;
    }

    &__card {
      margin-bottom: 25px;
      width: 100%;

      @include from(desktop) {
        width: 48%;
      }
    }
  }
</style>
