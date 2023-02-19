<template>
  <nav>    
    <v-navigation-drawer
      v-if="$vuetify.breakpoint.xsOnly"
      v-model="drawer"
      app
      clipped
      absolute
    >
      <v-list nav>
        <v-list-item v-if="$vuetify.breakpoint.xsOnly" link to="/" >
          <v-list-item-action>
            <v-icon>mdi-home</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="/">
          <v-list-item-action>
            <v-icon>mdi-home</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="/Contact">
          <v-list-item-action>
            <v-icon>mdi-book-open</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Contact</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="/Skills">
          <v-list-item-action>
            <v-icon>mdi-book</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Skills</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="/Works">
          <v-list-item-action>
            <v-icon>mdi-contacts</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Works</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    
    
    <v-app-bar app clipped-left >
    <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
    <v-toolbar 
    density="compact"
    dark
    >   
    <v-spacer></v-spacer> 
        <v-toolbar-title 
        class="ml-6 pr-6"
        show-arrows
        style="width:100 cursor: pointer" @click="$router.push('/')"
        >
        <v-toolbar-side-icon @click.stop="drawer = !drawer"></v-toolbar-side-icon>
        <span class="text-h4 text-decoration-underline goldrod--text" > Frimpong</span>
        </v-toolbar-title>

        <v-tabs
        v-if="$vuetify.breakpoint.lgOnly"
        align-with-title
        grow
        style="width: 20em"
        show-arrows
        center-active
        >
          <v-tab to="/Contact">Contact</v-tab>
          <v-tab to="/Skills">Skills</v-tab>
          <v-tab to="/Works">Works</v-tab>
        </v-tabs>
    
      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-github</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-linkedin</v-icon>
      </v-btn>

    </v-toolbar>
  </v-app-bar>
</nav>

</template>

<script>
  export default {
    data: () => ({
      drawer: null,
    }),    
    }
</script>



<style>
*{
  color:goldenrod;
  text-underline-position:below;
}

</style>


