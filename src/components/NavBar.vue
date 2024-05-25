<template>
  <div id="nav">
    <nav>
      <router-link to="/"> 
        <img src="" alt="Logo">
      </router-link>
      <router-link to="/">Home</router-link> |
      <router-link to="/pedidos">Pedidos</router-link>
    </nav>
    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>