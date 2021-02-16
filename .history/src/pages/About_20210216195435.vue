<template>
  <b-container fluid class="text-center p-0 m-0">
    <Navbar />
    <b-jumbotron
      header="Contents"
      lead=""
      header-tag="h2"
      fluid
      class="m-0"
      header-level="4"
    >
    </b-jumbotron>
    <h3>Side Nav Buttons</h3>
    <div id="mySidenav" class="sidenav">
      <a href="#" id="overview">Overview</a>
      <a href="#" id="domains">Domains</a>
      <a href="#" id="themes">Themes</a>
      <a href="#" id="projects">Projects</a>
    </div>
  </b-container>
</template>

<script lang="ts">
import { Vue, Component } from "@/utils/vue-imports";
import Navbar from "@/components/Navbar.vue";

@Component({
  name: "About",
  components: {
    Navbar,
  },
})
export default class About extends Vue {}
</script>

<style>
#mySidenav a {
  position: absolute;
  left: 10px;
  background-color: navy;
  border-radius: 5px;

  padding: 15px;
  width: 100px;
}

#mySidenav a:hover {
  left: 0;
}

#overview {
  top: 260px;
  visibility:unset;
}

#domains {
  top: 300px;
}

#themes {
  top: 340px;
}

#projects {
  top: 380px;
}
</style>
