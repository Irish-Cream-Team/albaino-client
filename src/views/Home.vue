<template>
  <div class="home">
    <h1 class="display-1">Hello Shavit, welcome back</h1>
    <v-card class="mx-auto" color="#43a047" dark max-width="400">
      <v-img gradient="to top right, rgba(55,236,186,.7), rgba(25,32,72,.7)">
        <v-card-title class="justify-center">
          <span class="headline font-weight-medium">My Projects</span>
        </v-card-title>

        <v-card-text class="headline font-weight-small">
        <v-hover>
          Aman Board
        </v-hover>
        </v-card-text>

        <v-card-text class="headline font-weight-small">
          Aman Board
        </v-card-text>

        <v-card-text class="headline font-weight-small">
          Aman Board
        </v-card-text>
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
