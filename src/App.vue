
<template>
  <NavBar></NavBar>
  <Main></Main>
  <Footer></Footer>

</template>

<script>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
import Main from './components/Main.vue';

export default {
  components: { NavBar, Footer, Main },
  data() {
    return
  }
}

</script>

<style scoped></style>
