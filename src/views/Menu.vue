<template>
  <div class="flex justify-between min-h-screen flex-col">
    <div class="">
      <Navbar></Navbar>
      <Hero></Hero>
      <Profile></Profile>
      <Skill></Skill>
    </div>
    <div class="">
      <Footer></Footer>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Navbar from "../components/Navbar.vue";
import Footer from "../components/Footer.vue";
import Hero from "../components/Hero.vue";
import Profile from "../components/Profile.vue";
import Skill from "../components/Skill.vue";

export default defineComponent({
  components: {
    Navbar,
    Footer,
    Hero,
    Profile,
    Skill,
  },

  data() {
    return {
      project: [
        {
          nama: "asqalani",
        },
        {
          nama: "Farish",
        },
      ],
    };
  },
});
</script>

<style></style>
