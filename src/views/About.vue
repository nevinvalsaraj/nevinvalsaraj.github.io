<template>
  <Header />
  <div class="about">
    <h1>About</h1>
    <p>
      Hello there!
      <br />I'm a software engineer at Microsoft.
      <br />I have the dubious honour of being a Linux-savvy MacBook-user in a world
      of Windows experts.
    </p>
    <p>
      I also love literature, but I keep subverting my own efforts in blogging
      by repeatedly rebuilding this website and blog with the year's flavor of
      JavaScript frameworks.
    </p>
    <p>
      This website is built using the wonderfully fast
      <a
        href="https://vuejs.org/"
        target="_blank"
        rel="noreferrer"
      >Vue.js</a>
      .
    </p>
    <router-link to="/">Back to home</router-link>
  </div>
</template>

<script>
import Header from "../components/Header.vue";

export default {
  name: "About",
  components: {
    Header,
  },
};
</script>

<style scoped>
.about {
  display: flex;
  flex-direction: column;
  text-align: center;
  font-weight: 100;
  color: #333;
  width: 50%;
}
.about a {
  color: #333;
}
.about p {
  font-size: 1.2rem;
  line-height: 1.4;
}

@media only screen and (max-width: 600px) {
  .about {
    width: 90%;
  }
  .about p {
    font-size: 0.9rem;
  }
}
</style>
