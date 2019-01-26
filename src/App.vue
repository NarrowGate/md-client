<template>
  <div class="columns">
    <div id="app" class="column mantra">
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

body {
  background: #d0d2d2;
  height: 100%;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
#nav {
  padding: 30px;
  background: #505d75;
  a {
    font-weight: bold;
    color: #2c3e50;
  }
  li {
    display: inline-block;
    cursor: pointer;
    padding: 0 10px;
    color:#fafafb;

    &:hover {
      color: #9c9693;
    }

    &.router-link-exact-active {
      color: #00aced;
    }
  }
}

.is-mantra {
  background:#ffffff;
  color:#4d5b73;
}

.mantra {
  .title {
    color: #00aced;
  }
}
</style>
