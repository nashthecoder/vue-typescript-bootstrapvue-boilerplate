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
#mySidenav {
  position: absolute;
  left: -60px;
  background-color: gray;
  border-radius: 0 5px 5px 0;
}

#overview {
  top: 20px;
  background-color: #4CAF50;
}

#domains {
  top: 80px;
  background-color: #2196F3; /* Blue */
}

#themes {
  top: 140px;
  background-color: #f44336; /* Red */
}

#projects {
  top: 200px;
  background-color: #555 /* Light Black */
}
</style>
