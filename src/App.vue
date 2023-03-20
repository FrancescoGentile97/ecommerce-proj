<template>
  <NavBar></NavBar>

  <Main></Main>
  
  <Footer></Footer>
</template>

<script>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
import Main from './components/Main.vue';
import { store } from './store';

export default {
  components: { NavBar, Footer, Main },
  data() {
    return{
      store,
    }
  }
}

</script>

<style lang="scss">
@use "./main.scss";
</style>
