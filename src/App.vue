<template>
  <div id="app" class="wrapper">
    <HeaderComponent title="404 NOT FOUND" />
    <div class="main">
      <ErrorComponent />
    </div>
    <FooterComponent :name="footer.name" :challenge="footer.challenge" />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import ErrorComponent from './components/ErrorComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    FooterComponent,
    ErrorComponent
  },
  data() {
    return {
      'footer': {
        'name': 'Carlos Santillan Espinoza',
        'challenge': 'DevChallenges.io'
      }
    }
  }
}
</script>

<style lang="scss">
@import './assets/scss/app'
</style>
