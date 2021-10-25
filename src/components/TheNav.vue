<template>
  <div id="nav">
    <router-link id="logo" to="/">FOREST</router-link>
    <div class="nav-left">
      <router-link to="/about">About</router-link>
      <a href="#">Contact</a>
      <fa id="cart-icon" :icon="['fas', 'bars']" />
    </div>
    <!-- <fa :icon="['fab', 'youtube']" /> -->
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#nav {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  padding: 1rem 3rem;
  color: #fff;

  a {
    color: white;
    text-decoration: none;
  }
}

#logo {
  font-size: 32px;
  color: white;
  font-family: 'Poppins', sans-serif;
  font-weight: 900;
  letter-spacing: 0.4rem;
  transition: all 0.2s ease;
}

#cart-icon {
  font-size: 24px;
  cursor: pointer;
  transition: all 0.2s ease;
  padding-bottom: 3px;

  &:hover {
    opacity: 0.5;
  }
}

.nav-left {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 300px;
  font-family: 'Yanone Kaffeesatz', sans-serif;
  font-size: 1.8rem;
  font-weight: 400;

  a {
    position: relative;
    transition: all 0.2s ease;

    &::after {
      content: '';
      width: 0%;
      height: 2px;
      position: absolute;
      bottom: 0;
      left: 50%;
      transform: translateX(-50%);
      border-radius: 99px;
      background: #fff;
      transition: all 0.4s;
    }

    &:hover::after {
      width: 75%;
    }
  }
}
</style>
