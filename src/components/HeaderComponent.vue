<template>
  <header class="header">
    <div class="container">
      <h1 class="header__title animate__animated animate__fadeIn">
        {{ title }}
      </h1>
    </div>
  </header>
</template>

<script>
export default {
    name: "HeaderComponent",
    props: [
      'title'
    ]
}
</script>