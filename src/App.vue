<template>
  <div>
    <NavBarComp />
    <router-view />
    <FooterComp/>
  </div>
</template>

<script>
import NavBarComp from "../src/components/NavBar.vue";
import FooterComp from '../src/components/Footer.vue';

export default {

  components: { NavBarComp, FooterComp }
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  text-decoration: none;

}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

img {
  width: 80px;
  float: left;
  top: 0;
  left: 0;
}

/*footer*/
footer {
  background-image: url("https://i.postimg.cc/bYxhhcJy/output-onlinepngtools-1-1.png");
  background-position: right;
  background-repeat: no-repeat;
  background-color: #619f67;
  color: black;
  font-size: 16px;
  margin-top: 50px;

}

footer * {
  font-family: "Poppins", sans-serif;
  box-sizing: border-box;
  border: none;
  outline: none;

}

.row {
  padding: 1em 1em;
}

.row.primary {
  display: grid;
  grid-template-columns: 2fr 1fr 1fr 2fr;
  align-items: stretch;
}

.column {
  width: 100%;
  display: flex;
  flex-direction: column;
  padding: 0 2em;
  min-height: 15em;
}

h3 {
  width: 100%;
  text-align: left;
  color: white;
  font-size: 1.4em;
  white-space: nowrap;
}

.info {
  list-style: none;
  display: flex;
  flex-direction: column;
  padding: 0;
  margin: 0;
}

.things:not(:first-child) {
  margin-top: 0.8em;
}

.info,
.things a {
  color: black;
  text-decoration: none;
}

.info,
.things a:hover {
  color: #23764a;
}

.about p {
  text-align: justify;
  line-height: 2;
  margin: 0;
}

.but,
.sub {
  font-size: 1em;
  padding: 1em;
  width: 100%;
  border-radius: 5px;
  margin-bottom: 5px;
}

.but {
  background-color: #6b9d56;
  color: black;
}

div.social {
  display: flex;
  justify-content: space-around;
  font-size: 2.4em;
  flex-direction: row;
  margin-top: 0.5em;
}

.social i {
  color: black
}

.copyright {
  padding: 0.3em 1em;

}

.footer-menu {
  float: left;
  margin-top: 10px;
}

.footer-menu a {
  color: black;
  padding: 6px;

  text-decoration: none;
}

.footer-menu a:hover {
  color: #619f67;
}

.copyright p {
  font-size: 0.9em;
  text-align: center;
  background-color: white;
  top: 50px;
}

@media screen and (max-width: 850px) {
  .row.primary {
    grid-template-columns: 1fr;
  }

}

.up {
  font-size: 2rem;

}

span {
  color: white;

}</style>
