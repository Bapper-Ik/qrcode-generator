<template>
  <div class="about mb-96">
    <div class="bg-green-100 max-w-full my-10 mx-3 px-5 py-6 text-left rounded-xl">

      <h1 class="text-slate font-bold font-serif text-2xl pb-5">About us</h1>

      <p class="text-lg font-sans leading-6 pb-2">This is Qr-Code Generator v1.0.1.</p>
      <span class="italic text-base text-red-400 capitalize ">warning !</span>
      <p class="text-lg font-sans pt-2"> To generate a Qr image you must have an internet connection before the image is gonna display out!</p>
    </div>
    
  </div>
  <Footer />
</template>

<script>
import Footer from "../components/Footer";

export default {
  name: 'About',
  components: {
    Footer,
  }
}
</script>
