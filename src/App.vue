<template>
  <div id="app" class="container">
    <nav class="navbar is-light" role="navigation" aria-label="dropdown navigation">
      <a class="navbar-item">
        <b>Vue CMS Gallery</b>
      </a>
    </nav>

    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.navbar {
  min-height: 3.25rem;
}

</style>
