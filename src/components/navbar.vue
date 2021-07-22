<template>
  <div class="navbar">
    <div class="sidebar-btn">
      <div class="line"></div>
      <div class="line"></div>
      <div class="line"></div>
    </div>
    <navbar-link v-for="(link, index) in links" :link="link" :key="index">
    </navbar-link>
  </div>
</template>

<script>
import navbarLink from "./navbarLink";
import("../css/navbar.css");
export default {
  components: {
    "navbar-link": navbarLink,
  },
  data() {
    return {
      //use vuex for the links
      links: [
        {
          name: "homepage",
          path: "/",
        },
      ],
    };
  },
};
</script>

<style>
@import "../src/css/navbar";
</style>