<template>
  <div class="page g-padding">
    <h2 class="page__title title">
      _MORE ABOUT ME
    </h2>
    <p class="page__paragraph paragraph--2">
      Im a Web Developer with almost 2 years of experience.  My core abilities are related to HTML, CSS, SCSS and Javascript, but I also have knowledge in React JS, Vue JS and their frameworks such as Gatsby Js, Next JS and Nuxt JS. Also I have experience with Styled components, Emotion JS, Storybook, Bootstrap and Rest Apis. I use Github to store some of my projects and because of that I know how to use Git.
    </p>
    <p class="page__paragraph paragraph--2">
      Currently  I am learning Graphql, Node JS and Typescript as one of my goals is to be a Full stack developer.
    </p>
    <p class="page__paragraph paragraph--2">
      I am a fast learner and enjoy creating new things, I prefer to work in a team environment as I believe it let me learn new things from my team members and also share my knowledge with them.
    </p>
    <p class="page__paragraph paragraph--2">
      I am eligible to work in South Korea as a full time worker legally and currently I am looking for a relocation there as my wife and baby are living in South Korea, both of them are Korean.
    </p>
    <Button text="Go back" class="page__button" to="/"/>
  </div>
</template>

<script>
    import Button from "../Button";

    export default {
      components: {
        Button
      }
    }
</script>

<style lang="scss">
  .page {
    align-items: flex-start;
    display: flex;
    flex-flow: column nowrap;
    justify-content: space-between;
    height: 90vh;
    width: 100vw;

    &__title {
      align-self: flex-start;
      color: $black;
    }

    &__paragraph {
      line-height: 20px;
      color: $black;
    }

    &__button {
      align-self: flex-start;
      border: 1px solid $black;
      color: $black;

      &:hover {
        background: black;
        color: $white;
      }
    }
  }
</style>
