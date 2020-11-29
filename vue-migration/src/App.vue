<template>
  <div id="app">
    <nav
      class="navbar sticky-top navbar-expand-md"
      role="navigation"
    >
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item mx-4">
            <router-link to="/">Home</router-link>
          </li>
          <li class="nav-item mx-4">
            <router-link to="/about">About Me</router-link>
          </li>
          <li class="nav-item mx-4">
            <router-link to="/work">Work</router-link>
          </li>
          <li class="nav-item mx-4">
            <router-link to="/contact">Contact Me</router-link>
          </li>
        </ul>
      </div>
    </nav>
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

@media (min-width: 768px) {
    .navbar-nav {
        float: none;
        margin: 0 auto;
        display: block;
        text-align: center;
      }
      
      .navbar-nav > li {
        display: inline-block;
        float: none;
      }
}

.navbar-nav a {
  color: #f4f7f7;
  text-decoration: none;
}

.navbar-nav a:hover {
  color: #f4f7f7;
  text-decoration: underline;
}

</style>