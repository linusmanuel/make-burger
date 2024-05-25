<template>
  <div id="main-banner">
    <h1>Make Your Burger</h1>
    <img src="" alt="">

  </div>
</template>

<script>
  export default {
    name: 'Banner'
  }
</script>

<style scoped>
  #main-banner {
    background-image: url('../assets/img/burger.jpg');
    background-position: center;
    background-size: cover;
    height: 500px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
  }

  #main-banner h1 {
    color: #fff;
    text-align: center;
    background-color: #222;
    padding: 30px;
  }
</style>