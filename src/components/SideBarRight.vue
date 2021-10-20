<template>
  <v-navigation-drawer app color="grey lighten-3" right width="270">
    <v-toolbar color="grey lighten-3" flat>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-badge bordered overlap color="red" dot>
          <v-icon>far fa-bell</v-icon>
        </v-badge>
      </v-btn>
      <v-badge bordered bottom color="teal" dot offset-x="10" offset-y="10">
        <v-avatar size="40" rounded>
          <v-img src="0.png" max-height="100" max-width="100"></v-img>
        </v-avatar>
      </v-badge>
      <v-btn icon>
        <v-icon>fas fa-ellipsis-v</v-icon>
      </v-btn>
    </v-toolbar>
    <v-toolbar class="pl-0 mt-5" flat color="grey lighten-8">
      <h3>My Orders</h3>
      <v-spacer></v-spacer>
      <h6 class="teal--text">Edit</h6>
    </v-toolbar>
    <v-app-bar flat color="rgba(0,0,0,0)" class="mt-n5">
      <v-btn fab x-small color="teal lighten-4" elevation="0">
        <v-icon color="teal">fas fa-clock</v-icon>
      </v-btn>
      <h5 class="ml-2 grey--text text--darken-2">17:30 PM</h5>
    </v-app-bar>

    <v-app-bar flat color="rgba(0,0,0,0)" class="mt-n5">
      <v-btn fab x-small color="teal lighten-4" elevation="0">
        <v-icon color="teal">fas fa-map-marker-alt</v-icon>
      </v-btn>
      <h5 class="ml-2 grey--text text--darken-2">29 Funzi Road, Nairobi</h5>
    </v-app-bar>

    <v-app-bar flat color="rgba(0,0,0,0)" class="mt-n5">
      <v-btn fab x-small color="teal lighten-4" elevation="0">
        <v-icon color="teal">fas fa-comment-dots</v-icon>
      </v-btn>
      <h5 class="ml-2 grey--text text--darken-2">Any Question?</h5>
    </v-app-bar>
    
    <v-divider></v-divider>

    <v-container>
      <v-row>
        <v-col cols="12" sm="3">
          <v-img src="0.png" max-height="50" max-width="50" contain class="mt-1 mr-1"></v-img>
        </v-col>
        <v-col cols="12" sm="3">
          <h6 class="ml-n6 grey--text text--darken-2">Chicken Salad</h6>
          <span class="grey--text text--lighten-1">987grams</span>
        </v-col>
        <v-col cols="12" sm="6">
          <v-chip class="ml-n5" color="teal" outlined text-color="black" small>
            <v-icon left x-small>
              fas fa-plus
            </v-icon>
            <v-divider vertical inset class="mr-1"></v-divider>
            1
            <v-divider vertical inset class="mr-1"></v-divider>
            <v-icon right x-small>
              fas fa-minus
            </v-icon>
          </v-chip>
          <strong class="ml-1 mr-1">$5.08</strong>
          <v-icon>
            fas fa-times
          </v-icon>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12" sm="3">
          <v-img src="2.png" max-height="50" max-width="50" contain class="mt-1 mr-1"></v-img>
        </v-col>
        <v-col cols="12" sm="3">
          <h6 class="ml-n6 grey--text text--darken-2">Miwa Chai</h6>
          <span class="grey--text text--lighten-1">2Kgs</span>
        </v-col>
        <v-col cols="12" sm="6">
          <v-chip class="ml-n5" color="teal" outlined text-color="black" small>
            <v-icon left x-small>
              fas fa-plus
            </v-icon>
            <v-divider vertical inset class="mr-1"></v-divider>
            1
            <v-divider vertical inset class="mr-1"></v-divider>
            <v-icon right x-small>
              fas fa-minus
            </v-icon>
          </v-chip>
          <strong class="ml-1 mr-1">$12.00</strong>
          <v-icon x-small>
            fas fa-times
          </v-icon>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12" sm="3">
          <v-img src="0.png" max-height="50" max-width="50" contain class="mt-1 mr-1"></v-img>
        </v-col>
        <v-col cols="12" sm="3">
          <h6 class="ml-n6 grey--text text--darken-2">Chicken Salad</h6>
          <span class="grey--text text--lighten-1">896Grms</span>
        </v-col>
        <v-col cols="12" sm="6">
          <v-chip class="ml-n5" color="teal" outlined text-color="black" small>
            <v-icon left x-small>
              fas fa-plus
            </v-icon>
            <v-divider vertical inset class="mr-1"></v-divider>
            1
            <v-divider vertical inset class="mr-1"></v-divider>
            <v-icon right x-small>
              fas fa-minus
            </v-icon>
          </v-chip>
          <strong class="ml-1 mr-1">$4.09</strong>
          <v-icon x-small>
            fas fa-times
          </v-icon>
        </v-col>
      </v-row>      
    </v-container>
    <div class="text-center">
      <v-btn class="px-12" outlined color="teal">Drag & Drop</v-btn>
    </div>
    <v-toolbar class="pl-0" flat color="grey lighten-3">
      <h3>Total</h3>
      <v-spacer></v-spacer>
      <h3>$15.98</h3>
    </v-toolbar>
    <div class="text-center">
      <v-btn class="px-15" rounded color="teal" dark>
        Checkout
      </v-btn>
    </div>
    <div class="text-center">
      <v-card elevation="2" class="mt-2 mx-2 pa-3">
        <v-container>
          <v-row>
            <v-col cols="12" sm="2">
              <v-icon color="blue" class=ml-n2>fab fa-cc-visa</v-icon>
            </v-col>
            <v-col cols="12" sm="2"><span class="caption text-9xl ml-n3">****</span></v-col>
            <v-col cols="12" sm="2"><span class="caption text-9xl ml-n5">****</span></v-col>
            <v-col cols="12" sm="2"><span class="caption text-9xl ml-n5">****</span></v-col>
            <v-col cols="12" sm="2"><span class="caption text-9xl ml-n5">5132</span></v-col>
            <v-col cols="12" sm="2"><v-icon small>fas fa-edit</v-icon></v-col>
          </v-row>
        </v-container>
      </v-card>
    </div>
  </v-navigation-drawer>
</template>

<script>
export default {

}
</script>

<style>

</style>