<template>
  <div id="app">
    <Header />
    <main>
      <router-view />
    </main>
  </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
  name: 'App',
  components: {
    Header,
  },
};
</script>

<style>
*:not(h1, h2, p, a, span, div) {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  color: #234;
  margin: 0;
  padding: 0;
}

main {
  margin: 2%;
}

ul {
  list-style: none;
}

a {
  color: black;
  font-weight: bold;
  text-decoration: none;
}

a.router-link-exact-active {
  color: #4b8;
}

a:visited {
  color: black;
}

img {
  max-width: 100%;
}

.container {
  max-width: 800px;
  margin: 0 auto;
}

.v-enter {
  opacity: 0;
  transform: translate3d(-20px, 0, 0);
}
.v-enter-active {
  opacity: 1;
  transition: all 0.3s;
}

.conteudo {
  display: grid;
  grid-template-columns: 1fr minmax(200px, 400px);
  grid-gap: 30px;
}

@media screen and (max-width: 800px) {
  .conteudo {
    grid-template-columns: 1fr;
  }
}
</style>
