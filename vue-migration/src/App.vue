<template>
  <div id="app">
     <nav class="navbar sticky-top navbar-expand-md heading-color-scheme" role="navigation">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
            aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
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

<style>

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

@import './assets/css/landing-page.css';
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Montserrat:wght@300;700&display=swap");
</style>
