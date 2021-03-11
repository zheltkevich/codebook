<template>
  <div id="app">
    <ul id="main-sections">
      <li><router-link to="/">Home</router-link> |</li>
      <li><router-link to="/about">About</router-link> |</li>
      <li><router-link to="/test">Test</router-link></li>
    </ul>
    <slot></slot>
  </div>
</template>

<style lang="scss">
#app {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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
