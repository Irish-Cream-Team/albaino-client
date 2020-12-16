<template>
  <v-app>
    <v-hover>
      <v-card-title
      slot-scope="{ hover }"
      :class="`${hover? 'class1': 'class2'}`">
      
        <v-app-bar absolute color="#43a047" dark>
          <template v-slot:img="{ props }">
            <v-img
              v-bind="props"
              gradient="to top right, rgba(55,236,186,.7), rgba(25,32,72,.7)">
            </v-img>
          </template>

          <v-app-bar-nav-icon></v-app-bar-nav-icon>

          <v-toolbar-title>YESODOT</v-toolbar-title>


        </v-app-bar>
      </v-card-title>
    </v-hover>
    
    <v-container style="height: 800px;"></v-container>

    <v-main>
      <router-view></router-view>
    </v-main>
    
  </v-app>
</template>




<script>

export default {
  name: 'App',
  data: () => ({
    //
  }),
};
</script>