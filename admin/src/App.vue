<template>
  <div id="app">
    <nav>
      <router-link to="/" tag="button">Publish</router-link>
      <router-link to="/manage" tag="button">Episodes</router-link>
      <router-link to="/users" tag="button">Users</router-link>
      <router-link to="/settings" tag="button">Settings</router-link>
      <button onclick="document.cookie = 'POGO_SESSION=;expires=Thu, 01 Jan 1970 00:00:01 GMT';window.location = '/'">Logout</button>
    </nav>
    <h1>Pogo LAUNCHPAD</h1>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
body {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  margin:0; padding:0;
}
h1,h2,h3,h4,h5 {
  font-weight: 400;
}
.podcastlist {
  padding-bottom: 10%;
}
#app {
  margin: 0 auto;
  padding: 0 2.0rem;
  position: relative;
  width: 60vw;
  height: 100%;
}
button, .button {
  margin-bottom: 10px;
  background-color: #397AD6;
  border: none;
  color: white;
  padding: 5px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  -webkit-transition:.52s;
    -moz-transition: .5s;
    -o-transition: .5s;
    -ms-transition: .5s;
    transition:.5s;
}
button:hover, .button:hover {
  background-color: #50B7D5;
}
footer {
  position: absolute;
  right: 0;
  bottom: 0;
  left: 0;
  padding: .25rem;
  color: #f9f9f9;
  background-color: #397AD6;
  text-align: center;
}
table {
  text-align: left;
  width: 100%;
}
nav a {
  margin-bottom: 10px;
  background-color: #397AD6;
  border: none;
  color: white;
  padding: 5px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  -webkit-transition:.52s;
    -moz-transition: .5s;
    -o-transition: .5s;
    -ms-transition: .5s;
    transition:.5s;
}
nav a:hover {
  background-color: #50B7D5;
}
.podcast {
  width:70%;
}
label {
  display: block;
}
hr {
  max-width: 40%;
}
.notifications {
  margin:0; padding:10px;
  font-size: 130%;
  height: 1.5vw;
  text-align: center;
}
.css {
  font-family: Monospace;
}
input[type=text], input[type=date], input[type=file], input[type=password],textarea, select {
  padding:10px;
  border-radius: 4px;
  box-sizing: border-box;
  border: 1px solid #397AD6;
}
.publish [type=text],
.publish input[type=date],
.publish input[type=file],
.publish input[type=password],
.publish textarea  {
  width: 100%;
}
.publish textarea {
  height: 30vh;
}

</style>
