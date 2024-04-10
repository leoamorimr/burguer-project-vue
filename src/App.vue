<template>
  <Navbar :logo="logo" :alt="app_name" />
  <router-view />
  <Footer />
</template>

<script>
import Footer from './components/Footer.vue';
import Navbar from './components/Navbar.vue';

export default {
  data() {
    return {
      logo: '/img/logo.png',
      app_name: 'Make Your Burguer'
    }
  },
  components: {
    Navbar,
    Footer
  }
}
</script>
<style>
* {
  font-family: Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main-container {
  margin: 50px;
  min-height: 250px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
