<template>
  <v-app id="app">
    <v-navigation-drawer v-model="drawer" app clipped>
      <!-- <v-list dense> -->
      <v-list-item two-line>
        <v-list-item-avatar>
          <img :src="'http://msuedu.ru/u/526/avatar3219.jpg'" />
        </v-list-item-avatar>
        <v-list-item-content class="text-left">
          <v-list-item-title class="font-weight-black">Sosiallink</v-list-item-title>
          <v-list-item-subtitle>Tom Udras</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
      <v-divider class="my-3"></v-divider>

      <v-list-item link to="Home">
        <v-list-item-action>
          <v-icon>mdi-home-circle</v-icon>
        </v-list-item-action>

        <v-list-item-content>
          <v-list-item-title class="text-left">Home page</v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-list-item link to="Login">
        <v-list-item-action>
          <v-icon>mdi-login</v-icon>
        </v-list-item-action>

        <v-list-item-content>
          <v-list-item-title class="text-left">Login</v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-list-item link>
        <v-list-item-action>
          <v-icon>mdi-account-multiple</v-icon>
        </v-list-item-action>
        <v-list-item-content>
          <v-list-item-title>Frends</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
      <v-list-item link>
        <v-list-item-action>
          <v-icon>mdi-account-search-outline</v-icon>
        </v-list-item-action>
        <v-list-item-content>
          <v-list-item-title>Fiend friend</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
      <!-- </v-list> -->
    </v-navigation-drawer>

    <v-app-bar app clipped-left>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title>Estrampava</v-toolbar-title>
    </v-app-bar>
    <v-footer app>
      <span>&copy; ceberpank</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  props: {
    source: String
  },
  data: () => ({
    drawer: null
  }),
  created() {
    this.$vuetify.theme.dark = true;
  }
};
</script>