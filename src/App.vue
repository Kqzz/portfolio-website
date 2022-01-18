<template>
  <NavBar />
  <Main></Main>
  <Projects></Projects>
  <Contact></Contact>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Main from "./components/Main.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";

export default {
  name: "App",
  components: {
    NavBar,
    Main,
    Projects,
    Contact,
  },
};
</script>

<style>
@import url("./styles/reset.css");

@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap");

#app {
  overflow-x: hidden;
  overflow-y: auto;
  font-family: "Poppins";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #181618;
  margin-top: 60px;
  margin-right: 0px;
  margin-left: 0px;
  scroll-behavior: smooth;
  padding-bottom: 3rem;
}

a {
  text-decoration: none;
}
a:hover {
  cursor: pointer;
}

.btn {
  font-size: 2.5rem;
  padding-right: 2rem;
  padding-left: 2rem;
  padding-top: 0.4rem;
  padding-bottom: 0.4rem;
  border-radius: 15px;
  margin-right: 1em;
  border: 2px solid #181618;
  text-align: center;
  color: #181618;
}
</style>
