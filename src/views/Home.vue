<template>
<v-app id="inspire">
  <SideBarLeft />
  <SideBarRight />
  <v-container>
    <v-toolbar flat>
      <v-row>
        <v-col cols="12" sm="10">
          <v-text-field label="Search" filled rounded dense solo flat background-color="grey lighten-3"></v-text-field>
        </v-col>
        <v-col cols="12" sm="2">
          <v-btn>
            <v-icon>fas fa-filter</v-icon>Filter
          </v-btn>
        </v-col>
      </v-row>
    </v-toolbar>
    <v-row class="mt-n9">
      <v-col cols="12" sm="6">
        <v-toolbar class="" flat>
          <h5>My Filters</h5>
          <v-icon class="ml-1" small>fas fa-car-side</v-icon>
          <h5 class="ml-1">First Meal</h5>
          <v-chip class="ma-2" color="teal" text-color="white" dense>
            <v-avatar left>
              <v-icon>fas fa-running</v-icon>
            </v-avatar>
            After Training
          </v-chip>
          <v-spacer></v-spacer>
          <h6 class="teal-text">ADD</h6>
        </v-toolbar>
      </v-col>
      <v-col cols="12" sm="6">
        <v-toolbar class="" flat>
          <h5>popular Filters</h5>
          <v-icon class="ml-1" small>fas fa-child</v-icon>
          <h5 class="ml-1">Slim Waist</h5>
          <v-spacer></v-spacer>
          <v-icon class="ml-1">fas fa-birthday-cake</v-icon>
          <h5 class="ml-1">Diet</h5>
        </v-toolbar>
      </v-col>
    </v-row>
    <v-toolbar class="pl-0 mt-n7" flat>
      <h4>234</h4>
      <h4 class="grey--text text--lighten-1 ml-2">Meals Found</h4>
      <v-spacer></v-spacer>
      <h4 class="grey--text text--lighten-1">Sorted by</h4>
      <h4 class="ml-1">Recommended</h4>
      <v-icon class="ml-1">fas fa-chevron-down</v-icon>
    </v-toolbar>
    <v-row class="mt-n6">


      
      <v-col cols="12" sm="4">
        <v-hover v-dlot="{hover}" open-delay="200">
          <v-card color="red lighten-5" :elevation="hover ? 16: 2">
            <v-app-bar flat color="rgba(0,0,0,0)">
              <v-chip class="ma-2" color="black" text-color="white" dense>
                <v-avatar left>
                  <v-icon color="yellow">fas fa-star</v-icon>
                </v-avatar>
                4.2
              </v-chip>
              <v-spacer></v-spacer>
              <v-btn fab x-small color="white"><v-icon>far fa-heart</v-icon></v-btn>
            </v-app-bar>
            <div class="d-flex flex-column justify-space-between align-center">
              <v-img src="0.png" max-height="100" max-width="100"></v-img>
            </div>
            <v-app-bar flat color="rgba(0,0,0,0)">
              <h5 class="ml-1 grey--text text-lighten-3">Chicken Salad</h5>
              <v-chip class="ma-2" color="grey lighten-3" text-color="red" dense>
                250g
              </v-chip>
            </v-app-bar>
            <h5 class="ml-5 mt-n5">$4.98</h5>
          </v-card>
        </v-hover>
      </v-col>
      


    </v-row>
  </v-container>
</v-app>
</template>

<script>
  import SideBarLeft from '../components/SideBarLeft'
  import SideBarRight from '../components/SideBarRight'

  export default {
    name: 'Home',

    components: {
      SideBarLeft,
      SideBarRight
    },
  }
</script>
