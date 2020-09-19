<template>
  <div class="container">
    <div class="hero">
      <div class="hero__img animate__animated animate__zoomIn">
        <img :src="imageUrl" :alt="error.status">
      </div>
      <div class="hero__info">
        <h2 class="hero__title animate__animated animate__zoomIn">{{ error.title }}</h2>
        <p class="hero__description animate__animated animate__zoomIn">{{ error.description }}</p>
        <a href="#" class="hero__btn animate__animated animate__zoomIn">{{ error.btn }}</a>
      </div>
    </div>    
  </div>
</template>

<script>
export default {
    name: "ErrorComponent",
    data(){
      return{
        error: {
          'status': "404 Logo",
          'image': 'Scarecrow.png',
          'title': "I have bad news for you",
          'description': "The page you are looking for might be removed or is temporarily unavailable",
          'btn': 'Back to Homepage'
        }
      }
    },
    computed: {
      imageUrl(){
        return require(`../assets/img/${this.error.image}`)
      }
    }
}
</script>