<template>
  <div>
    <header>
      <nav class="shift navbar jutify-content-between navbar-light bg-light">
        <div class="main-logo">
          <n-link class="navbar-brand" to="/">
            <icon-base viewBox="0 0 512 512" icon-name="fake">
              <icon-fake />
            </icon-base>
          </n-link>
        </div>
        <div class="list-nav">
          <ul class="h-100 m-0 p-0 d-flex list-unstyled justify-content-end align-items-center">
            <li class="h-100">
              <n-link to="/index">Lorem ipsum dolor</n-link>
            </li>
            <li class="h-100">
              <n-link to="/index">Suspendisse sed</n-link>
            </li>
            <li class="h-100">
              <n-link to="/index">Sed at purus eget</n-link>
            </li>
            <li class="h-100">
              <n-link to="/index">Praesent dignissim</n-link>
            </li>
            <li class="h-100">
              <n-link to="#">Etiam aliquam dui</n-link>
            </li>
          </ul>
        </div>
        <div class="search-bar">
          <form class="form-inline my-2 my-lg-0">
            <input class="form-control mr-sm-2" type="search" placeholder="Mot clés de recherche" />
            <button class="btn btn-outline-success my-2 my-sm-0" type="submit">
              <icon-base viewBox="0 0 512.005 512.005" icon-name="search">
                <icon-search />
              </icon-base>
            </button>
          </form>
        </div>
      </nav>
    </header>
  </div>
</template>

<script>
import IconBase from "../components/IconBase.vue";
import IconFake from "../components/icons/IconFake.vue";
import IconSearch from "../components/icons/IconSearch.vue";
export default {
  name: "AppHeader",
  components: {
    IconBase,
    IconFake,
    IconSearch,
  },
};
</script>

<style scoped>
.navbar {
  flex-wrap: nowrap;
  padding: 0 1em !important;
}
.navbar-brand img {
  width: 70px;
}
.form-inline {
  flex-flow: nowrap;
}
ul li a,
ul li a:hover {
  text-decoration: none;
}
nav ul li a {
  display: block;
  text-align: center;
  font-size: 0.8em;
  padding: 15px;
  color: #433c35;
  font-weight: 800;
  text-transform: uppercase;
}
nav ul li a,
nav ul li a:after,
nav ul li a:before {
  transition: all 0.5s;
}
nav.shift ul li a {
  position: relative;
  z-index: 1;
}
nav.shift ul li a:hover {
  color: #003900;
}
nav.shift ul li a:after {
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  margin: auto;
  width: 100%;
  height: 1px;
  content: ".";
  color: transparent;
  background: #93d50a;
  visibility: none;
  opacity: 0;
  z-index: -1;
}
nav.shift ul li a:hover:after {
  opacity: 1;
  visibility: visible;
  height: 100%;
}
nav.main-logo {
  flex-basis: 10%;
}
nav.list-nav {
  flex-basis: 50%;
}

/** Search bar */

nav.search-bar {
  flex-basis: 40%;
}
.search-bar input,
.search-bar button,
.search-bar button:hover {
  border-radius: 0;
  border-color: #ced4da;
  background-color: #ffffff;
  color: #433c35;
}
.search-bar input {
  min-width: 200px;
  margin-right: 0 !important;
  border-right: 0;
}
.search-bar button {
  border-left: 0;
  color: #433c35;
}
.form-control,
.search-bar button {
  font-size: 0.8em;
}
</style>