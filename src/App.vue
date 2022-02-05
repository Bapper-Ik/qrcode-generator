<template>
  <div id="app" class="pb-4 mx-auto">
    <Header />
   <Output  />
   <Footer />
  </div>
   
</template>

<script>
import './assets/tailwind.css';
import Header from "./components/layout/Header";
import Output from "./components/Output";
import Footer from "./components/Footer";
export default {
  name: 'App',
  components: {
    Header,
    Output,
    Footer
  }
}
</script>

<style>
* {
  box-sizing: border-box;
  padding:0;
  margin: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1,4;
}

</style>
