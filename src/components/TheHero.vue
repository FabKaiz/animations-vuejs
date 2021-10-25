<template>
  <div class="container">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
      <fa :icon="['fas', 'carrot']" />
      <fa :icon="['fab', 'youtube']" />
    </div>
    <h2>tertr</h2>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
.container {
  width: 100%;
  height: 100vh;
  // background-image: linear-gradient(rgba(0, 0, 0, 0.3), transparent),
  //   url(../assets/images/Forest-large.jpg);
  background-size: cover;
  background-position: center;
  // padding: 0 8%;
  position: relative;
}

</style>
