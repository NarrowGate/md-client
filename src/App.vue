<template>

<div class="container">
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
    </div>
  </div>
  <footer class="has-text-centered">
    <p>© 2019 Mantra Driving</p>
  </footer>
</div>

</template>

<style lang="scss">

html {
  height: auto;
  min-height:100vh;
  padding:0;
}

body {
  background: url('../public/img/mantra_bg_long.jpg') no-repeat top;
  background-size: cover;
  min-height:100vh;
  height: inherit;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
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
    color:#d2c6b4;

    &:hover {
      color: #9c9693;
    }

    &.router-link-exact-active {
      color: white;
      background: #e75500;
      padding: 5px 10px;
    }
  }
}



.mantra {
  .title {
    color: white;
    font-size:150px;
    margin-bottom:0 !important;
    padding-bottom:0;
  }
  .subtitle {
    font-size:72px;
  }
  .container {
    padding: 1rem;
    min-height: 30vh;
  }
  p {
    padding: 1rem;
    color: white;
    font-size: 18px;
  }
  input, textarea {
    border-radius: 0;
    border-color: #7bccec;
  }

  .title {
    font-weight: normal;
  }
}

.bgC_1 {
  background:#e75500;
}

.bgC_2 {
  background:#4b4a48;
}

.bgC_3 {
  background:#d3c6b5;
}

footer {
  color: #d2c6b4;
  height: 100px;;
  line-height: 100px;
}

// =======================
// Home
.is-mantra {
  color:#4d5b73;
}

.is-mantra h2 {
  color: white;
  padding: 1rem;
  font-size: 36px;
}

.is-mantra .bgC_3 h2, .is-mantra .bgC_3 p  {
  color:#5d2814 !important;
}

// =======================
// Resources

// =======================
// Location

// =======================
// Packages

.packages .column {
    flex-basis: 200px;
}

.packages .card {
    background: rgba(75, 74, 72, 0.5)
}

.packages .card-header-title {
    color:#5d2814;
    background: #d3c6b5;
    flex-grow:0;
    font-size:20px;
    font-weight:normal;
}
.packages .buy {
    display: flex;
    justify-content: center;
    padding: 1rem;
}

.buy a {
    font-size: 2rem;
    color:#e85400;
    display: block;
    width: 100%;
    text-align:center;
    transition: background .75s, color .75s;
}

.buy a:hover {
    background: #e85400;
    color: white;
}

// =======================
// Buy Packages

.sidebar {
    background: #4b4a48;
}

.sidebar h2 {
    font-size: 25px;
    color: #d2c6b4;
}
.mantraForm {
    background: rgba(75, 74, 72, 0.5);
    color:#d2c6b4;
}

.mantraForm .label {
    color: white;
    font-weight: normal;
}

.mantraForm input, .mantraForm .select select, .mantraForm .textarea {
    border: 1px solid #e75500;
    background-color: transparent;
    color:#d2c6b4;
    border-radius: 0;
}

.mantraForm select {
    width: 100%
}

.paypal-button, .mantraForm button {
    width:100%;
    height: 50px;
    background: #e75500 !important;
    border-radius: 0;
}

// =======================
// Testimony

// =======================
// Contact Form

.inputError input {
    border: red 1px solid;
}

.error {
    display: none;
}
.inputError .error {
    display: block;
}

</style>
