<template>
  <header>
    <nav>
      <div class="logo">
        <router-link to="/">Techno</router-link>
      </div>
      <ul>
        <li><router-link to="/cursos">Cursos</router-link></li>
        <li><router-link to="/contato">Contato</router-link></li>
      </ul>
    </nav>
  </header>
</template>

<script>
// Imports

export default {
  name: 'Header',
};
</script>

<style scoped>
header {
  background: #234;
}

header a {
  color: white;
}
nav {
  max-width: 800px;
  margin: 0 auto;
  display: flex;
  align-content: space-between;
  padding: 20px;
}

.logo {
  flex: 1;
}

.logo a {
  font-size: 1.2rem;
  color: white;
}

ul li {
  display: inline-block;
}
ul li + li {
  margin-left: 20px;
}

li a {
  padding: 0 10px;
}
</style>
