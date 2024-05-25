<template>
  <nav id="nav">
      <router-link to="/" id="url-logo"> 
        <img src="../assets/img/logo.png" :alt="alt" id="logo">
      </router-link>
      <router-link to="/">Home</router-link>
      <router-link to="/pedidos">Pedidos</router-link>
    </nav>
</template>

<script>
export default {
  name: 'NavBar',
  props: ['logo', 'alt']
}
</script>

<style scoped>
  #nav {
    background-color: #222;
    padding: 15px 50px;
    border-bottom: solid 4px #111;
    display: flex;
    justify-content: flex-end;
    align-items: center;
}

#nav #url-logo {
  width: 40px;
  margin: auto;
  margin-left: 0;
}

#logo {
  width: 40px;
}

#nav a {
  color: #fcba03;
  text-decoration: none;
  margin: 12px;
  transition: .5s;
}

#nav a:hover {
  color: #fff;
}
</style>