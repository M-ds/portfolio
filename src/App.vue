<template>
  <nav>
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-link to="/work">Work</router-link>
  </nav>
  <router-view />
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
  float: right;
  width: 10rem;

  a {
    font-weight: bold;
    color: #2c3e50;
    background-color: #eee;
    display: block;
    padding: 12px;
    text-decoration: none;

    &:hover {
      background-color: yellow;
    }

    &.router-link-exact-active {
      color: #42b983;
      background-color: red;
    }
  }
}
</style>
