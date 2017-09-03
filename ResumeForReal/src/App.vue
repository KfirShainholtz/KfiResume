<template>
  <div id="app">
    <div class="resume_left_half">
      <div id="resume_image">
      </div>

      <div class="resume_profile_name">
        <h1>Kfir Shainholtz</h1>
      </div>
    </div>

    <div class="resume_right_half">
      <img src="./assets/logo.png">
      <h1>{{ msg }}</h1>
      <h2>Essential Links</h2>
      <ul>
        <li>
          <a href="https://vuejs.org" target="_blank">Core Docs</a>
        </li>
        <li>
          <a href="https://forum.vuejs.org" target="_blank">Forum</a>
        </li>
        <li>
          <a href="https://gitter.im/vuejs/vue" target="_blank">Gitter Chat</a>
        </li>
        <li>
          <a href="https://twitter.com/vuejs" target="_blank">Twitter</a>
        </li>
      </ul>
      <h2>Ecosystem</h2>
      <ul>
        <li>
          <a href="http://router.vuejs.org/" target="_blank">vue-router</a>
        </li>
        <li>
          <a href="http://vuex.vuejs.org/" target="_blank">vuex</a>
        </li>
        <li>
          <a href="http://vue-loader.vuejs.org/" target="_blank">vue-loader</a>
        </li>
        <li>
          <a href="https://github.com/vuejs/awesome-vue" target="_blank">awesome-vue</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

body {
  height: 90%;
  background: linear-gradient(90deg, #2ecc71 50%, #FFFFFF 50%);
}

div#resume_image {
  margin-left: auto;
  margin-right: auto;
  width: 8em;
  background-size: cover;
  border-radius: 50%;
  width: 8em;
  height: 8em;
  background-image: url(assets/profile.jpg);
  background-repeat: no-repeat;
  transition: background-image 0.5s;
}

div#resume_image:hover {
  background-image: url(assets/linkedin.png);
}

.resume_left_half {
  flex: 1;
  padding: 1rem;
  grid-column: 1;
}

.resume_right_half {
  flex: 1;
  padding: 1rem;
  grid-column: 2;
}

#app {
  display: flex;
}

.resume_profile_name {
  font-family: Lato;
  color: white;
  font-weight:100;
}
</style>
