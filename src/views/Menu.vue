<template>
  <div class="flex justify-between min-h-screen flex-col">
    <div class="">
      <Navbar></Navbar>
      <Hero></Hero>
      <Profile></Profile>
      <Skill></Skill>
      <Project></Project>
      <Contact></Contact>
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
import Project from "../components/Project.vue";
import Contact from "../components/Contact.vue";

export default defineComponent({
  components: {
    Navbar,
    Footer,
    Hero,
    Profile,
    Skill,
    Project,
    Contact,
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
