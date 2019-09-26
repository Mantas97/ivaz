<template>
  <section class="container">
    <div>
      <logo />
      <h1 class="title">
        ivaz-project
      </h1>
      <h2 class="subtitle">
        ivaz project
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green"
        >Documentation</a>
        <i class="material-icons white-text">error_outline</i>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey"
        >GitHub</a>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style lang="scss">

$font-stack: 'RobotoBold';
$primary-color: rgb(224, 0, 0);

body {
  font: 100% $font-stack;
  color: $primary-color !important;
}

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  // font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
  //   'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: $primary-color;
  font-family: $font-stack;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
