<template>
  <div id="app">
    <b-navbar toggleable="sm" type="dark" class="navbar" sticky>
      <b-navbar-toggle target="navbar-toggle-collapse"></b-navbar-toggle>
      <b-collapse id="navbar-toggle-collapse" is-nav>
        <b-navbar-nav class="mx-auto navbar-nav" fill>
          <b-nav-item class="mx-4"> 
            <router-link to="/">Home</router-link> 
          </b-nav-item>
          <b-nav-item class="mx-4">
            <router-link to="/about">About Me</router-link>
          </b-nav-item>
          <b-nav-item class="mx-4">
            <router-link to="/work">Work</router-link>
          </b-nav-item>
          <b-nav-item class="mx-4">
            <router-link to="/contact">Contact Me</router-link>
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <router-view />
  </div>
</template>

<style scoped>
.navbar {
  background-color: #34495e;
  color: #f4f7f7;
}

.navbar-toggler-icon {
  background-image: url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 30 30' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath stroke='rgba(255, 255, 255, 1)' stroke-width='2' stroke-linecap='round' stroke-miterlimit='10' d='M4 7h22M4 15h22M4 23h22'/%3E%3C/svg%3E");
}

.navbar-nav a {
  color: #f4f7f7;
  text-decoration: none;
}

.navbar-nav a:hover {
  color: #aacfd0;
}

.navbar a.router-link-exact-active {
  color: #5da0a2;
  font-weight: bold;
}
</style>
