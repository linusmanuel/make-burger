<template>
  <div>
    <Banner />
    <div class="main-container">
      <h1>Monte seu hamburguer:</h1>
      <p>Formulario</p>
    </div>
  </div>
</template>

<script>
import Banner from '../components/Banner.vue'

export default {
  name: 'HomeView',
  components: {
    Banner,
  }
}
</script>
