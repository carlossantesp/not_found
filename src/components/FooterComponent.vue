<template>
  <footer class="footer">
    <div class="container">
      <p class="footer__copy animate__animated animate__fadeIn">
        {{ name }} &copy; {{ challenge }}
      </p>
    </div>
  </footer>
</template>

<script>
export default {
    name: "FooterComponent",
    props: [
      'name',
      'challenge'
    ]
}
</script>