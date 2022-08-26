<template>
  <v-app>
  <v-container>
    <v-card
      class="mx-auto overflow-hidden"
      height="auto"
    >

      <v-app-bar
        app
        dark
      >
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
        <v-toolbar-title>KASH-KIKU</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn icon href="https://www.instagram.com/kash.kiku">
          <v-icon>mdi-instagram</v-icon>
        </v-btn>
      </v-app-bar>
      
      <v-navigation-drawer
        v-model="drawer"
        fixed
        temporary
      >
        <v-list
          nav
          dense
        >
          <v-list-item-group>
            <v-list-item>
              <v-list-item-title>
                <router-link to="/">Home</router-link> 
              </v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title>
                <router-link to="/about">About</router-link>
              </v-list-item-title>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-navigation-drawer>
     </v-card>
  <div id="cards">
  <router-view />
  </div>
  </v-container>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      drawer: false
    }
  }
}
</script>
 
<style>

#cards {
    margin-top: 56px;
  }


.mdi-instagram {
  background: radial-gradient(
    circle at 30% 107%,
    #fdf497 0%,
    #fdf497 5%,
    #fd5949 45%,
    #d6249f 60%,
    #285aeb 90%
  );
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
}

</style>