<template>
  <main id="main">
    <div id="header">
      <Header />
    </div>
    <div id="banner">
      <Banner />
    </div>
    <div id="content">
      <Content />
    </div>
    <div class="aside">
      <Aside />
    </div>
    <div class="footer">
      <Footer />
    </div>
  </main>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Header from "./components/Header.vue";
import Banner from "./components/Banner.vue";
import Content from "./components/Content.vue";
import Aside from "./components/Asside.vue";
import Footer from "./components/Footer.vue";

export default defineComponent({
  name: "App",
  components: {
    Header,
    Banner,
    Content,
    Aside,
    Footer,
  },
});
</script>

<style>
* {
  margin: 0%;
  text-decoration: none;
  color: white;
}
</style>
