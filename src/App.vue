<template>
  <div id="app">
    <Header />
    <FormReg />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import FormReg from "./components/FormReg.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "app",
  components: {
    Header,
    FormReg,
    Footer
  }
};
</script>

<style>
body {
  margin: 0;
  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto,
    Helvetica Neue, Arial, Noto Sans, sans-serif, Apple Color Emoji,
    Segoe UI Emoji, Segoe UI Symbol, Noto Color Emoji;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5;
  color: #212529;
  text-align: left;
  background-color: #fff;
}
</style>
