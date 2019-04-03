<template>
  <div id="app">
    <!-- Navigation -->

  <nav class="navbar navbar-expand-lg navbar-dark fixed-top" id="mainNav">
      <div class="container">
        <a class="navbar-brand js-scroll-trigger" href="#page-top">Coffee Junkie</a>
        <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
          <i class="fas fa-bars"></i>
        </button>
        <div class="collapse navbar-collapse" id="navbarResponsive">
          <ul class="navbar-nav text-uppercase ml-auto">
            <li class="nav-item">
              <a class="nav-link js-scroll-trigger" href="#menu">Menu</a>
            </li>
            <li class="nav-item">
              <a class="nav-link js-scroll-trigger" href="#about">About</a>
            </li>
            <li class="nav-item">
              <a class="nav-link js-scroll-trigger" href="#team">Team</a>
            </li>
            <li class="nav-item">
              <a class="nav-link js-scroll-trigger" href="#contact">Contact</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  
    <!-- Header -->

    <Header></Header>
  
    <!-- Menu -->
    
    <Menu></Menu>
  
    <!-- About -->

    <About></About>

    <!-- Team -->

    <Team></Team>
  
    <!-- Contact -->

    <Contact></Contact>
  
    <!-- Footer -->

    <Footer></Footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Menu from "./components/Pages/Menu.vue";
import About from "./components/Pages/About.vue";
import Team from "./components/Pages/Team.vue";
import Contact from "./components/Pages/Contact.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "app",
  components: {
    Header,
    Menu,
    About,
    Team,
    Contact,
    Footer
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
