<template>
  <nav class="navbar">
    <v-app-bar app class="toolbar" color="#43a047">
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(55,236,186,.7), rgba(25,32,72,.7)"
        >
        </v-img>
      </template>
      <v-toolbar-title class="white--text">
        <span>Hello Shavit</span>
      </v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items>
        <v-btn depressed icon tile large color="white" class="px-10"
          ><v-icon>mdi-home</v-icon></v-btn
        >
        <v-btn depressed icon tile large color="white" class="px-10"
          ><v-icon>mdi-autorenew</v-icon></v-btn
        >
        <v-btn depressed icon tile large color="white" class="px-10"
          ><v-icon>mdi-cloud-download</v-icon></v-btn
        >
        <v-btn depressed icon tile large color="white" class="px-10"
          ><v-icon>mdi-file-document</v-icon></v-btn
        >
      </v-toolbar-items>

      <v-spacer></v-spacer>

      <v-toolbar-title class="text-uppercase white--text">
        <span class="font-weight-light">Yeso</span>
        <span>Dot</span>
      </v-toolbar-title>
    </v-app-bar>
  </nav>
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
</style>
