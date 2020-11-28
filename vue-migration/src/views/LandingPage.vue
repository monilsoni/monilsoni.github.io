<template>
<div>
    <Heading />
    <Main />
    <Footer />
</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Heading from "@/components/Heading.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";

@Component({
  components: {
    Heading,
    Main,
    Footer
  }
})
export default class LandingPage extends Vue {}
</script>