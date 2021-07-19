<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
html {
  scroll-behavior: smooth;
  transition: 400ms;
}
html::-webkit-scrollbar {
  display: none;
}
#app {
  overflow: hidden;
  max-width: 426px;
  margin: 0 auto;
  font-family: "Source Sans Pro", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  margin: 0 !important;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
