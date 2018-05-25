<template>
  <div id="app">
    <app-nav-bar></app-nav-bar>
    <app-banner></app-banner>
    <app-features></app-features>
    <app-team></app-team>
    <app-filler></app-filler>
    <app-about></app-about>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Banner from './components/Banner.vue'
import Features from './components/Features.vue'
import Filler from './components/Filler.vue'
import Team from './components/Team.vue'
import NavBar from './components/NavBar.vue'
import About from './components/About.vue'
import Footer from './components/Footer.vue'



export default {
  name: 'App',
  components: {
    appBanner: Banner,
    appFeatures: Features,
    appFiller: Filler,
    appTeam: Team,
    appNavBar: NavBar,
    appAbout: About,
    appFooter: Footer
}
}
</script>

<style lang="scss">
  @import './styles/custom_bootstrap.scss';
  @import '../node_modules/bootstrap/scss/bootstrap.scss';
</style>

<style>
body {
  margin-top: 60px;
}
/*h1, h2, h3, h4, h5 {
  font-family: 'Roboto Condensed', sans-serif;
}*/
.height-100 {
  min-height: 100vh;
}
.height-80 {
  min-height: 80vh;
}
.height-60 {
  min-height: 60vh;
}
.height-50 {
  min-height: 50vh;
}
.height-40 {
  min-height: 40vh;
}

#filler {
  background:  linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('./assets/food.jpg');
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
