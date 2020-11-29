<template>
  <div class="home">
    <Heading />
    <div id="about-me" class="container-fluid">
      <div class="row section dark-blue text-center">
        <div class="col" style="margin: auto;">
          <img src="./../assets/images/monil.png" alt="My Profile Picture" />
          <h2>Hello!</h2>
          <p>
            I'm a software dev engineer at Amazon, India. I love watching movies
            and T.V. series. I also like sketching, reading, and (sometimes)
            writing. I also like talking about minimalism and productivity.
          </p>
        </div>
      </div>
    </div>
    <div id="projects" class="container-fluid">
      <div class="row section light-blue text-center">
        <div class="col" style="margin: auto">
          <h2>Projects</h2>
          <p>
            I am familiar with web development, as well as android development.
            You can check out
            <a class="link" href="https://github.com/monilSoni"
              >my GitHub profile</a
            >
            and
            <a
              class="link"
              href="https://drive.google.com/file/d/1yGWxtctbBk3ObBaHaXNN9x3RTxpMtxbS/view?usp=sharing"
              >my resume</a
            >. I am a casual Vim user - that is I prefer using Vim keybindings
            in whatever IDE I use but, I am not yet at the stage where I can
            make Vim my IDE (someday, hopefully).
          </p>
        </div>
      </div>
    </div>
    <div id="contact-me" class="container-fluid">
      <div class="row section dark-blue text-center">
        <div class="col" style="margin: auto;">
          <h2>Contact Me</h2>
          <p>
            Is there something I can help you with? Or do you want to just chat
            over a cup of coffee? Please feel free to reach out :)
          </p>
          <a href="mailto:monilsoni99@gmail.com" style="margin-top: 20px"
            >Message Me!</a
          >
        </div>
      </div>
    </div>    
    <Footer />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Heading from "@/components/Heading.vue";
import Footer from "@/components/Footer.vue";

@Component({
  components: {
    Heading,
    Footer
  }
})
export default class Home extends Vue {}
</script>

<style scoped>

.section {
  color: #212d3b;
  padding: 50px;
  min-height: 600px;
}

.section.dark-blue {
  background-color: #5da0a2;
}

.section.light-blue {
  background-color: #aacfd0;
}

</style>