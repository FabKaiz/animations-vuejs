<template>
  <div class="container">
    <TheNav></TheNav>
    <div class="text-content">
      <p>Welcome to</p>
      <h1>FOREST</h1>
      <h3>
        Here you can book amazing roadtrip around the world to visit beautiful
        forest!
      </h3>

      <div class="row">
        <a href="#">Click here to see more 🌲</a>
        <span></span>
      </div>
    </div>
  </div>
</template>

<script>
import TheNav from './TheNav.vue';

export default {
  components: {
    TheNav,
  },
};
</script>

<style lang="scss" scoped>
.container {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0.12),
      rgba(28, 46, 35, 0.671)
    ),
    url(../assets/images/Forest-large.jpg);
  background-size: cover;
  background-position: center;
  // padding: 0 8%;
  position: relative;
}

.text-content {
  font-family: 'Yanone Kaffeesatz', sans-serif;
  color: #fff;
  position: absolute;
  bottom: 8%;
  left: 8%;

  p {
    font-size: 70px;
    font-weight: 600;
    margin: 0;
  }

  h1 {
    font-family: 'Poppins', sans-serif;
    font-size: 220px;
    line-height: 160px;
    margin: 0 0 0 -10px;
    color: transparent;
    -webkit-text-stroke: 1px #fff;
    background: url(../assets/images/back.png);
    background-clip: text;
    -webkit-background-clip: text;
    background-position: 0 0;
    animation: background 50s linear infinite;
  }

  @keyframes background {
    100% {
      background-position: 2000px 0;
    }
  }

  h3 {
    font-size: 32px;
    font-weight: 400;
  }
}

.row {
  display: flex;
  align-items: center;

  a {
    color: #fff;
    text-decoration: none;
    padding: 10px 20px;
    margin-right: 20px;
    border: 1px solid #fff;
    font-size: 24px;
    transition: all 0.2s;

    &:hover {
      background-color: rgba(255, 255, 255, 0.7);
      border: 1px solid transparent;
      color: #000;
    }
  }
}
</style>
