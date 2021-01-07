<template>
  <div class="home">
    <v-card
      id="myProjectsWindow"
      class="mx-auto"
      color="#43a047"
      dark
      max-width="400"
    >
      <v-img gradient="to top right, rgba(55,236,186,1), rgba(25,32,72,.7)">
        <v-card-title class="justify-space-between">
          <span id="myProjectsHeadline" class="headline font-weight-medium"
            >My Projects</span
          >
          <v-btn depressed icon tile large color="white" @click="counter"
            ><v-icon>mdi-plus</v-icon></v-btn
          >
        </v-card-title>

        <v-card-title
          id="projectsWindowHeadlines"
          class="justify-space-between"
        >
          <span class="headline font-weight-small">Name</span>
          <span class="headline font-weight-small">Version</span>
        </v-card-title>

        <div id="textOutline" class="d-flex flex-column align-start">
          <v-btn
            text
            x-large
            class="text-capitalize headline d-flex justify-space-between font-weight-bold"
            min-width="100%"
          >
            Aman Board
            <div>1</div></v-btn
          >
          <v-btn
            text
            x-large
            class="text-capitalize headline d-flex justify-space-between font-weight-bold"
            min-width="100%"
          >
            Aman Board
            <div>3.2</div></v-btn
          >
          <v-btn
            text
            x-large
            class="text-capitalize headline d-flex justify-space-between font-weight-bold"
            min-width="100%"
          >
            Aman Board
            <div>1.2</div></v-btn
          >
          <v-btn
            text
            x-large
            class="text-capitalize headline d-flex justify-space-between font-weight-bold"
            min-width="100%"
          >
            Aman Board
            <div>2</div></v-btn
          >
        </div>
      </v-img>
    </v-card>
  </div>
</template>

<script>
import { mapGetters } from "vuex";

export default {
  data() {
    return {
      hover: false,
    };
  },
  computed: {
    ...mapGetters(["counter"]),
  },
};
</script>

<style scoped>
#myProjectsWindow {
  margin-top: 8%;
}
#textOutline {
  -webkit-text-stroke: 0.4px black;
}
#projectsWindowHeadlines {
  margin-left: 3%;
  margin-right: 2.5%;
}
#myProjectsHeadline {
  margin-left: auto;
  margin-right: 23%;
}
</style>