<template>
  <div id="app" class="wrapper">
    <HeaderComponent />
    <ErrorComponent />
    <FooterComponent />
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
  }
}
</script>

<style lang="scss">
@import './assets/scss/app'
</style>
