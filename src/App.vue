<template>
  <div id="app">
    <NavBar :logo="logo_src" :alt="app_name" />
    
    <!-- Aplica a classe que cresce e empurra o footer -->
    <main class="main-content">
      <router-view />
    </main>

    <Footer />
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    Footer
  },
  data() {
    return {
      logo_src: "img/logo.png",
      app_name: "Make your Burger"
    };
  }
}
</script>

<style>
html, body {
  margin: 0;
  padding: 0;
  height: 100%;
  font-family: Helvetica;
  box-sizing: border-box;
}

#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.main-content {
  flex: 1;
  margin: 50px;
}

h1 {
  color: #222;
  font-size: 42px;
  margin-bottom: 30px;
  text-align: center;
}
</style>
