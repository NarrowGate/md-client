<template>
  <div class="columns">
    <div id="app" class="column">
      <div id="nav">
        <ul>
          <router-link tag="li" to="/">My Driving School</router-link>    
          <router-link tag="li" to="/resources">Resourses</router-link>
          <router-link tag="li" to="/location">Location</router-link>
          <router-link tag="li" to="/packages">Packages</router-link>
          <router-link tag="li" to="/testimony">Testimony</router-link>
          <router-link tag="li" to="/contact">Contact</router-link>    
        </ul>
      </div>
      <router-view/>

      <footer>
        <p>Footer Text</p>
      </footer>
    </div>
  </div>
</template>

<style lang="scss">

html, body {
  height: 100%;
}

body {
  background: #e2aab6;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
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
  }
  li {
    display: inline-block;
    cursor: pointer;
    padding: 0 10px;

    &:hover {
      color: #209cee;
    }

    &.router-link-exact-active {
      color: #209cee;
    }
  }
}
</style>
