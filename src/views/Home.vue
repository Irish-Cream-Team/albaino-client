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
        <v-card-title class="justify-center">
          <span class="headline font-weight-medium">My Projects</span>
        </v-card-title>
        <div id="textOutline" class="d-flex flex-column align-start">
          <v-btn
            text
            x-large
            class="text-capitalize headline d-flex justify-space-between font-weight-bold"
            min-width="100%"
          >
            Aman Board
            <div>Version 1</div></v-btn
          >
          <v-btn
            text
            x-large
            class="text-capitalize headline d-flex justify-space-between font-weight-bold"
            min-width="100%"
          >
            Aman Board
            <div>Version 3.2</div></v-btn
          >
          <v-btn
            text
            x-large
            class="text-capitalize headline d-flex justify-space-between font-weight-bold"
            min-width="100%"
          >
            Aman Board
            <div>Version 1.2</div></v-btn
          >
          <v-btn
            text
            x-large
            class="text-capitalize headline d-flex justify-space-between font-weight-bold"
            min-width="100%"
          >
            Aman Board
            <div>Version 2</div></v-btn
          >
        </div>
      </v-img>
    </v-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      hover: false,
    };
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
</style>